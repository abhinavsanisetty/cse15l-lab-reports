# *Chosen command: grep*

# Command Line Option/Alternative 1: ‘-v’ 

**Example 1:**

Code block of command:
```grep -v ".txt" find-results.txt```

Code block of output:
```
written_2/
written_2/non-fiction
written_2/non-fiction/OUP
written_2/non-fiction/OUP/Abernathy
written_2/non-fiction/OUP/Berk
written_2/non-fiction/OUP/Castro
written_2/non-fiction/OUP/Fletcher
written_2/non-fiction/OUP/Kauffman
written_2/non-fiction/OUP/Rybczynski
written_2/travel_guides
written_2/travel_guides/berlitz1
written_2/travel_guides/berlitz2
```
What is it doing, and why is it useful?

Before running this command I first used the find command and saved the results to ‘find-results.txt’ the find command I used was find `written_2/ > find-results.txt`. This command will search for all lines in the file ‘find-results.txt’  that do not contain the string “.txt”. This option is basically used to invert the results of grep, so instead of finding all the lines that do have the string “.txt”, it finds all the lines that do not have that string. This command is useful because it lets you return only the lines that dont have a certain string with just one command.

**Example 2-**

Code block of command:
```grep -v "travel_guides" find-results.txt ```

Code block of output:
```
written_2/
written_2/non-fiction
written_2/non-fiction/OUP
written_2/non-fiction/OUP/Abernathy
written_2/non-fiction/OUP/Abernathy/ch1.txt
written_2/non-fiction/OUP/Abernathy/ch14.txt
written_2/non-fiction/OUP/Abernathy/ch15.txt
written_2/non-fiction/OUP/Abernathy/ch2.txt
written_2/non-fiction/OUP/Abernathy/ch3.txt
written_2/non-fiction/OUP/Abernathy/ch6.txt
written_2/non-fiction/OUP/Abernathy/ch7.txt
written_2/non-fiction/OUP/Abernathy/ch8.txt
written_2/non-fiction/OUP/Abernathy/ch9.txt
written_2/non-fiction/OUP/Berk
written_2/non-fiction/OUP/Berk/CH4.txt
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Berk/ch2.txt
written_2/non-fiction/OUP/Berk/ch7.txt
written_2/non-fiction/OUP/Castro
written_2/non-fiction/OUP/Castro/chA.txt
written_2/non-fiction/OUP/Castro/chB.txt
written_2/non-fiction/OUP/Castro/chC.txt
written_2/non-fiction/OUP/Castro/chL.txt
written_2/non-fiction/OUP/Castro/chM.txt
written_2/non-fiction/OUP/Castro/chN.txt
written_2/non-fiction/OUP/Castro/chO.txt
written_2/non-fiction/OUP/Castro/chP.txt
written_2/non-fiction/OUP/Castro/chQ.txt
written_2/non-fiction/OUP/Castro/chR.txt
written_2/non-fiction/OUP/Castro/chV.txt
written_2/non-fiction/OUP/Castro/chW.txt
written_2/non-fiction/OUP/Castro/chY.txt
written_2/non-fiction/OUP/Castro/chZ.txt
written_2/non-fiction/OUP/Fletcher
written_2/non-fiction/OUP/Fletcher/ch1.txt
written_2/non-fiction/OUP/Fletcher/ch10.txt
written_2/non-fiction/OUP/Fletcher/ch2.txt
written_2/non-fiction/OUP/Fletcher/ch5.txt
written_2/non-fiction/OUP/Fletcher/ch6.txt
written_2/non-fiction/OUP/Fletcher/ch9.txt
written_2/non-fiction/OUP/Kauffman
written_2/non-fiction/OUP/Kauffman/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch10.txt
written_2/non-fiction/OUP/Kauffman/ch3.txt
written_2/non-fiction/OUP/Kauffman/ch4.txt
written_2/non-fiction/OUP/Kauffman/ch5.txt
written_2/non-fiction/OUP/Kauffman/ch6.txt
written_2/non-fiction/OUP/Kauffman/ch7.txt
written_2/non-fiction/OUP/Kauffman/ch8.txt
written_2/non-fiction/OUP/Kauffman/ch9.txt
written_2/non-fiction/OUP/Rybczynski
written_2/non-fiction/OUP/Rybczynski/ch1.txt
written_2/non-fiction/OUP/Rybczynski/ch2.txt
written_2/non-fiction/OUP/Rybczynski/ch3.txt
written_2/find-results.txt
```
What is it doing, and why is it useful?

Before running this command I first used the find command and saved the results to ‘find-results.txt’ the find command I used was find `written_2/ > find-results.txt`. This command will search for all lines in the file ‘find-results.txt’  that do not contain the string “travel_guides”. This option is basically used to invert the results of grep, so instead of finding all the lines that do have the string “travel_guides”, it finds all the lines that do not have that string. This command is useful because it lets you return only the lines that dont have a certain string with just one command.

Source: I used a ChatGPT search to find and learn about this command

## Command Line Option/Alternative 2: ‘-n’

**Example 1-**

Code block of command:
```grep -n "History" find-results.txt ```

Code block of output:
```
71:written_2/travel_guides/berlitz1/HistoryDublin.txt
72:written_2/travel_guides/berlitz1/HistoryEdinburgh.txt
73:written_2/travel_guides/berlitz1/HistoryEgypt.txt
74:written_2/travel_guides/berlitz1/HistoryFWI.txt
75:written_2/travel_guides/berlitz1/HistoryFrance.txt
76:written_2/travel_guides/berlitz1/HistoryGreek.txt
77:written_2/travel_guides/berlitz1/HistoryHawaii.txt
78:written_2/travel_guides/berlitz1/HistoryHongKong.txt
79:written_2/travel_guides/berlitz1/HistoryIbiza.txt
80:written_2/travel_guides/berlitz1/HistoryIndia.txt
81:written_2/travel_guides/berlitz1/HistoryIsrael.txt
82:written_2/travel_guides/berlitz1/HistoryIstanbul.txt
83:written_2/travel_guides/berlitz1/HistoryItaly.txt
84:written_2/travel_guides/berlitz1/HistoryJamaica.txt
85:written_2/travel_guides/berlitz1/HistoryJapan.txt
86:written_2/travel_guides/berlitz1/HistoryJerusalem.txt
87:written_2/travel_guides/berlitz1/HistoryLakeDistrict.txt
88:written_2/travel_guides/berlitz1/HistoryLasVegas.txt
89:written_2/travel_guides/berlitz1/HistoryMadeira.txt
90:written_2/travel_guides/berlitz1/HistoryMadrid.txt
91:written_2/travel_guides/berlitz1/HistoryMalaysia.txt
92:written_2/travel_guides/berlitz1/HistoryMallorca.txt
159:written_2/travel_guides/berlitz2/Algarve-History.txt
163:written_2/travel_guides/berlitz2/Amsterdam-History.txt
167:written_2/travel_guides/berlitz2/Athens-History.txt
171:written_2/travel_guides/berlitz2/Bahamas-History.txt
175:written_2/travel_guides/berlitz2/Bali-History.txt
178:written_2/travel_guides/berlitz2/Barcelona-History.txt
181:written_2/travel_guides/berlitz2/Beijing-History.txt
184:written_2/travel_guides/berlitz2/Berlin-History.txt
191:written_2/travel_guides/berlitz2/Budapest-History.txt
194:written_2/travel_guides/berlitz2/California-History.txt
197:written_2/travel_guides/berlitz2/Canada-History.txt
199:written_2/travel_guides/berlitz2/CanaryIslands-History.txt
202:written_2/travel_guides/berlitz2/Cancun-History.txt
205:written_2/travel_guides/berlitz2/China-History.txt
208:written_2/travel_guides/berlitz2/Costa-History.txt
211:written_2/travel_guides/berlitz2/CostaBlanca-History.txt
213:written_2/travel_guides/berlitz2/Crete-History.txt
217:written_2/travel_guides/berlitz2/Cuba-History.txt
220:written_2/travel_guides/berlitz2/Nepal-History.txt
223:written_2/travel_guides/berlitz2/NewOrleans-History.txt
226:written_2/travel_guides/berlitz2/Poland-History.txt
228:written_2/travel_guides/berlitz2/Portugal-History.txt
231:written_2/travel_guides/berlitz2/PuertoRico-History.txt
234:written_2/travel_guides/berlitz2/Vallarta-History.txt
```
What is it doing, and why is it useful?

Before running this command I first used the find command and saved the results to ‘find-results.txt’ the find command I used was find `written_2/ > find-results.txt`. This command will search for all lines in the file ‘find-results.txt’ that contain the string “History”, and it will also provide the line numbers for these lines. This command is useful because it lets you find all the lines with a string but it also tells you all of the line numbers so you know exactly where in the file each of these lines are located.

**Example 2-**

Code block of command:
```grep -n "Portugal" find-results.txt```

Code block of output:
```
228:written_2/travel_guides/berlitz2/Portugal-History.txt
229:written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt
230:written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt
```
What is it doing, and why is it useful?

Before running this command I first used the find command and saved the results to ‘find-results.txt’ the find command I used was find `written_2/ > find-results.txt`. This command will search for all lines in the file ‘find-results.txt’ that contain the string “Portugal”, and it will also provide the line numbers for these lines. This command is useful because it lets you find all the lines with a string but it also tells you all of the line numbers so you know exactly where in the file each of these lines are located.

Source: I used a ChatGPT search to find and learn about this command

## Command Line Option/Alternative 3: ‘-c’

**Example 1-**

Code block of command:
```grep -c "History" find-results.txt```

Code block of output:

```46```

What is it doing, and why is it useful?

Before running this command I first used the find command and saved the results to ‘find-results.txt’ the find command I used was find `written_2/ > find-results.txt`. This command will search for all lines in the file ‘find-results.txt’ that contain the string “History”, but rather than returning every line that has this string it instead counts how many lines have the string and returns the count instead. This command it useful because it lets you find the lines with a certain and count how many lines there in just one singular command.

**Example 2-**

Code block of command:
```grep -c "France" find-results.txt```

Code block of output:

```4```

What is it doing, and why is it useful?

Before running this command I first used the find command and saved the results to ‘find-results.txt’ the find command I used was find `written_2/ > find-results.txt`. This command will search for all lines in the file ‘find-results.txt’ that contain the string “France”, but rather than returning every line that has this string it instead counts how many lines have the string and returns the count instead. This command it useful because it lets you find the lines with a certain and count how many lines there in just one singular command.

Source: I used a ChatGPT search to find and learn about this command

## Command Line Option/Alternative 4: ‘-w’

**Example 1-**

Code block of command:
```grep -w -c "water" WhereToFrance.txt ```

Code block of output:

```15```

What is it doing, and why is it useful?

This option will search for all lines in the file ‘WhereToFrance.txt’ that contain the string “water”, but it will only match whole words that exactly match the search pattern and wont count partial words or words that contain the search pattern as a substring. For example in this case, it will only match the instance where it finds the string “water”, but it will ignore words like “waterfall” or “watery” since they are not an exact match for the whole word and only contain the pattern as a substring. This option is useful since it lets you avoid partial matches or matches on substrings and lets you only find the exact matches.

**Example 2-**

Code block of command:
```grep -w -c "old" WhereToFrance.txt ```

Code block of output:

```69```

What is it doing, and why is it useful?

This option will search for all lines in the file ‘WhereToFrance.txt’ that contain the string “old”, but it will only match whole words that exactly match the search pattern and wont count partial words or words that contain the search pattern as a substring. For example in this case, it will only match the instance where it finds the string “old”, but it will ignore words like “older” or “fold” since they are not an exact match for the whole word and only contain the pattern as a substring. This option is useful since it lets you avoid partial matches or matches on substrings and lets you only find the exact matches.

Source: I used a ChatGPT search to find and learn about this command

