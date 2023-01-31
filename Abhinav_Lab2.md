# Part 1

Code for server: 

```
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
   // The one bit of state on the server: a number that will be manipulated by
   // various requests.
   String s = "";

   public String handleRequest(URI url) {
       if (url.getPath().equals("/"))
       {
           return "";
       }
       else{
           System.out.println("Path: " + url.getPath());
           if (url.getPath().contains("/add-message")) {
               String[] parameters = url.getQuery().split("=");
               if (parameters[0].equals("s")) {
                   s += ("\n" + parameters[1]);
                   return s;
               }
           }
           return "404 Not Found!";
       }
   }
}


class StringServer {
   public static void main(String[] args) throws IOException {
       if (args.length == 0) {
           System.out.println("Missing port number! Try any number between 1024 to 49151");
           return;
       }

       int port = Integer.parseInt(args[0]);

       Server.start(port, new Handler());
   }
}

```

Screenshot 1:
![Message 1](Message1.png)

Here, the handleRequest method is the one being called. The only parameter that is taken in by this method is the url of the server. However, some of the other values are also modified during this screenshot. There is an array that is used to store the message that the user enters using “add-message”, and that changes to store the string “hello”. The string variable that holds all of the messages is also modified to also include the string “hello”, and it is put on a new line.

Screenshot 2:
![Message 2](Message2.png)

Here, the handleRequest method is the one being called. The only parameter that is taken in by this method is the url of the server. However, some of the other values are also modified during this screenshot. There is an array that is used to store the message that the user enters using “add-message”, and that changes to store the string “How’s your day going”. The string variable that holds all of the messages is also modified to also include the string “How’s your day going”, and it is put on a new line. So now the string variables has the string “Hello”, and then on a new line it has “How’s your day going”

## Part 2

Failure-Inducing input:
A failure-inducing input for the buggy program, as a JUnit test and any associated code (write it as a code block in Markdown)

An input that doesn’t induce a failure, as a JUnit test and any associated code (write it as a code block in Markdown)

The symptom, as the output of running the tests (provide it as a screenshot of running JUnit with at least the two inputs above)

The bug, as the before-and-after code change required to fix it (as two code blocks in Markdown)

Briefly describe why the fix addresses the issue.




