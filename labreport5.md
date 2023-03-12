# Lab report 5 
---
The lab report in which I will be discussing is lab report 3. Lab report 3 to me wasnt necessarily the most "fun" but was the most informational. Because of this, it is my favorite lab. In lab report 3, I researched the `grep` command and the many various ways to use it. In this report, I will be researching another command and that will be `find`. 

 - Example 1: The first command that I will be demonstrating is, `find -name`. Source: [Link](https://openai.com/blog/chatgpt)
   - Input 1: 
   ``` 
   find written_2/ -name "ch1.txt"
   ```
   - Output 1: 
   ``` 
   written_2/non-fiction/OUP/Abernathy/ch1.txt
   written_2/non-fiction/OUP/Berk/ch1.txt
   written_2/non-fiction/OUP/Fletcher/ch1.txt
   written_2/non-fiction/OUP/Kauffman/ch1.txt
   written_2/non-fiction/OUP/Rybczynski/ch1.txt
   ```
   - Input 2: 
   ``` 
   find written_2/ -name "ch1.txt"
   ```
   - Output 2: 
   ``` 
   written_2/non-fiction/OUP/Abernathy/ch2.txt
   written_2/non-fiction/OUP/Berk/ch2.txt
   written_2/non-fiction/OUP/Fletcher/ch2.txt
   written_2/non-fiction/OUP/Rybczynski/ch2.txt
   ```
    - The, `find -name` command can be used by the user to find a specifc file name. As shown in inputs 1 and 2, the user can input the file that they are exclusively looking for and, `find (directory) -name "(file)"` will display it. 
 
  - Example 2: The second command is, `find -mtime`. Source: [Link](https://unix.stackexchange.com/questions/529058/find-type-d-mtime-1-only-shows-one-file-in-a-4-day-span)
    - Input 1: 
    ```
    find written_2/ -mtime -40 -type f
    ```
    - Output 1: (output was too long so I had to shorten it. The output should show all the files because no changes had been made. Since this is the case, it would show all the files because the last time a change would have been made was when cloning it.)
    ```
    written_2/non-fiction/OUP/Abernathy/ch1.txt
    written_2/non-fiction/OUP/Abernathy/ch14.txt
    written_2/non-fiction/OUP/Abernathy/ch15.txt
    written_2/non-fiction/OUP/Abernathy/ch2.txt
    written_2/non-fiction/OUP/Abernathy/ch3.txt
    written_2/non-fiction/OUP/Abernathy/ch6.txt
    written_2/non-fiction/OUP/Abernathy/ch7.txt
    written_2/non-fiction/OUP/Abernathy/ch8.txt
    written_2/non-fiction/OUP/Abernathy/ch9.txt
    written_2/non-fiction/OUP/Berk/ch1.txt
    written_2/non-fiction/OUP/Berk/ch2.txt
    written_2/non-fiction/OUP/Berk/CH4.txt
    ```
    - Input 2: 
    ```
    find written_2/ -mtime -40 -type d
    ```
    - Output 2: 
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
    - The `find -mtime` commands allows the user to see the changes that have been made to a file and or directory within a certain amount of days. The, `find (directory) -mtime -(day) -type d` command allows the user to see the directories in which changes have been made to within a certain span of days. The, `find (directory) -mtime -(day) -type f` command shows which files had been changed based on the amount of days the user puts. 
  - Example 3: The third command is, `find -user`. 
    - Input 1: 
    ```
    find written_2/ -type d -user jtdng
    ```
    - Output 1:
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
    - Input 2: 
    ```
    find written_2/ -type f -user jtdng
    ```
    - Output 2: (output it too long so I shortened it.) 
    ```
    written_2/non-fiction/OUP/Abernathy/ch1.txt
    written_2/non-fiction/OUP/Abernathy/ch14.txt
    written_2/non-fiction/OUP/Abernathy/ch15.txt
    written_2/non-fiction/OUP/Abernathy/ch2.txt
    written_2/non-fiction/OUP/Abernathy/ch3.txt
    written_2/non-fiction/OUP/Abernathy/ch6.txt
    written_2/non-fiction/OUP/Abernathy/ch7.txt
    written_2/non-fiction/OUP/Abernathy/ch8.txt
    written_2/non-fiction/OUP/Abernathy/ch9.txt
    written_2/non-fiction/OUP/Berk/ch1.txt
    written_2/non-fiction/OUP/Berk/ch2.txt
    written_2/non-fiction/OUP/Berk/CH4.txt
    written_2/non-fiction/OUP/Berk/ch7.txt
    written_2/non-fiction/OUP/Castro/chA.txt
    written_2/non-fiction/OUP/Castro/chB.txt
    written_2/non-fiction/OUP/Castro/chC.txt
    ```
    - The `find -user` command lets the user find the files and or directories owned by that user specifc person. To find the directories that the user owns, the command, `find (directory) -type d -user (username)` shows all directories the user has. Because I haad specified which directories I owned in the written_2 directory, it showed directories in written_2. If I wanted to see all the directories I owned on my personal computer, the user could just put "." inplace of written_2 to see what directories that own. The, `find (directory) -type f -user (username)` command shows the user what files they own. Like the other command if the user doesnt specify which directory they want to see the files in which they own, it will show all files that the user owns. Since I specified the files in which I own in written_2 it only shows the files in written_2.
 - Example 4, the last command is, `find -empty`.
    
  
    
    
