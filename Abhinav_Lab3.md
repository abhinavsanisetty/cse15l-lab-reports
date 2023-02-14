# *Chosen command: find* **

Command Line Option/Alternative 1: ‘-type’ 

Example 1:
Code block of command
find written_2/non-fiction/OUP/ -type f
Code block of output
written_2/non-fiction/OUP//Berk/ch2.txt
written_2/non-fiction/OUP//Berk/ch1.txt
written_2/non-fiction/OUP//Berk/CH4.txt
written_2/non-fiction/OUP//Berk/ch7.txt
written_2/non-fiction/OUP//Abernathy/ch2.txt
written_2/non-fiction/OUP//Abernathy/ch3.txt
written_2/non-fiction/OUP//Abernathy/ch1.txt
written_2/non-fiction/OUP//Abernathy/ch7.txt
written_2/non-fiction/OUP//Abernathy/ch6.txt
written_2/non-fiction/OUP//Abernathy/ch8.txt
written_2/non-fiction/OUP//Abernathy/ch9.txt
written_2/non-fiction/OUP//Abernathy/ch15.txt
written_2/non-fiction/OUP//Abernathy/ch14.txt
written_2/non-fiction/OUP//Rybczynski/ch2.txt
written_2/non-fiction/OUP//Rybczynski/ch3.txt
written_2/non-fiction/OUP//Rybczynski/ch1.txt
written_2/non-fiction/OUP//Kauffman/ch3.txt
written_2/non-fiction/OUP//Kauffman/ch1.txt
written_2/non-fiction/OUP//Kauffman/ch4.txt
written_2/non-fiction/OUP//Kauffman/ch5.txt
written_2/non-fiction/OUP//Kauffman/ch7.txt
written_2/non-fiction/OUP//Kauffman/ch6.txt
written_2/non-fiction/OUP//Kauffman/ch8.txt
written_2/non-fiction/OUP//Kauffman/ch9.txt
written_2/non-fiction/OUP//Kauffman/ch10.txt
written_2/non-fiction/OUP//Fletcher/ch2.txt
written_2/non-fiction/OUP//Fletcher/ch1.txt
written_2/non-fiction/OUP//Fletcher/ch5.txt
written_2/non-fiction/OUP//Fletcher/ch6.txt
written_2/non-fiction/OUP//Fletcher/ch9.txt
written_2/non-fiction/OUP//Fletcher/ch10.txt
written_2/non-fiction/OUP//Castro/chR.txt
written_2/non-fiction/OUP//Castro/chP.txt
written_2/non-fiction/OUP//Castro/chQ.txt
written_2/non-fiction/OUP//Castro/chB.txt
written_2/non-fiction/OUP//Castro/chC.txt
written_2/non-fiction/OUP//Castro/chA.txt
written_2/non-fiction/OUP//Castro/chV.txt
written_2/non-fiction/OUP//Castro/chW.txt
written_2/non-fiction/OUP//Castro/chM.txt
written_2/non-fiction/OUP//Castro/chZ.txt
written_2/non-fiction/OUP//Castro/chL.txt
written_2/non-fiction/OUP//Castro/chN.txt
written_2/non-fiction/OUP//Castro/chY.txt
written_2/non-fiction/OUP//Castro/chO.txt

What is it doing, and why is it useful?
This command will search for all regular files in the directory ‘/written_2/non-fiction/OUP//’ and its subdirectories. This command is useful because it lets you return only the regular files (and not any directories, symbolic links, etc) within the specified directory using only 1 command.
Example 2-
Code block of command
find written_2/non-fiction/OUP/ -type d
Code block of output
written_2/non-fiction/OUP/
written_2/non-fiction/OUP//Berk
written_2/non-fiction/OUP//Abernathy
written_2/non-fiction/OUP//Rybczynski
written_2/non-fiction/OUP//Kauffman
written_2/non-fiction/OUP//Fletcher
written_2/non-fiction/OUP//Castro
What is it doing, and why is it useful?
This command will search for all directories in the directory ‘/written_2/non-fiction/OUP//’ and its subdirectories. This command is useful because it lets you return only the directories (and not any files, symbolic links, etc) within the specified directory using only 1 command.
Source:
ChatGPT

Command Line Option/Alternative 2: ‘-size’

Example 1-
Code block of command
find written_2/non-fiction/OUP/ -size -8k

Code block of output

written_2/non-fiction/OUP/
written_2/non-fiction/OUP//Berk
written_2/non-fiction/OUP//Abernathy
written_2/non-fiction/OUP//Rybczynski
written_2/non-fiction/OUP//Kauffman
written_2/non-fiction/OUP//Fletcher
written_2/non-fiction/OUP//Castro
written_2/non-fiction/OUP//Castro/chW.txt
written_2/non-fiction/OUP//Castro/chZ.txt
written_2/non-fiction/OUP//Castro/chY.txt

What is it doing, and why is it useful?
This command will find all files in the directory ‘written_2/non-fiction/OUP/’ that are smaller than 8 kilobytes. This is useful because you can use it to find all of the files that are less than a certain size.
Example 2-
Code block of command
find written_2/non-fiction/OUP/ -size +100k
Code block of output
written_2/non-fiction/OUP//Berk/ch2.txt
written_2/non-fiction/OUP//Berk/CH4.txt
What is it doing, and why is it useful?
This command will find all files in the directory ‘written_2/non-fiction/OUP/’ that are bigger than 100 kilobytes. This is useful because you can use it to find all of the files that are bigger than a certain size.
Source:
ChatGPT

Command Line Option/Alternative 3: ‘-delete’

Example 1-
Code block of command
find written_2/non-fiction/OUP/Castro -name "*.txt" -delete
Code block of output
*There is no output for this command*
What is it doing, and why is it useful?
This command will delete the files that match the specified criteria of the find command, in this case it will find all of the files with a ‘.txt’ extension in the directory ‘written_2/non-fiction/OUP/Castro’ and its subdirectories and delete them. This command is useful because you can delete all of the files that you find.
Example 2-
Code block of command
find written_2/non-fiction/OUP/Berk -name "*.txt" -delete
Code block of output
*There is no output for this command*
What is it doing, and why is it useful?
This command will find all of the files with a ‘.txt’ extension in the directory ‘written_2/non-fiction/OUP/Berk’ and its subdirectories and delete them. This command is useful because you can delete all of the files that you find.
Source:
ChatGPT

Command Line Option/Alternative 4: ‘-exec’

Example 1-
Code block of command
find written_2/non-fiction/OUP/Kauffman/ -name "*.txt" -exec wc {} \;
Code block of output
     144   13373   80544 written_2/non-fiction/OUP/Kauffman//ch3.txt
     148   10562   65578 written_2/non-fiction/OUP/Kauffman//ch1.txt
     125   12136   74448 written_2/non-fiction/OUP/Kauffman//ch4.txt
      62    4446   27196 written_2/non-fiction/OUP/Kauffman//ch5.txt
     101    8081   50095 written_2/non-fiction/OUP/Kauffman//ch7.txt
     124    9999   61513 written_2/non-fiction/OUP/Kauffman//ch6.txt
     236   16905   99145 written_2/non-fiction/OUP/Kauffman//ch8.txt
     178   14165   86220 written_2/non-fiction/OUP/Kauffman//ch9.txt
     132   10345   64908 written_2/non-fiction/OUP/Kauffman//ch10.txt
What is it doing, and why is it useful?
This command will find all the files with a ‘.txt’ extension in the directory ‘written_2/non-fiction/OUP/Kauffman/’ and its subdirectories, and then run the ‘wc’ command on each file. This is useful because you can find files and call ‘wc’ on them using just one command.
Example 2-
Code block of command
find written_2/non-fiction/OUP/Kauffman/ -name "*.txt" -exec tail -1 {} \;









Code block of output











What is it doing, and why is it useful?
This command will find all the files with a ‘.txt’ extension in the directory ‘written_2/non-fiction/OUP/Kauffman/’ and its subdirectories, and then run the ‘tail -n’ command on each file. This is useful because you can find files and call ‘tail -n’ on them using just one command.
Source:
ChatGPT

