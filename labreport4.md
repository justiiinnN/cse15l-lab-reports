# Lab Report 4 
--- 
 - In this report, I will be going through the steps in which I took to complete the task. 


 - Part 1: 
    - The first task was to delete the fork of the repository that had been previously cloned. The reason for this is to start fresh. 
       - To delete the repository in the terminal, the command needed to be used is, ***rm -rf lab7***.  
      
 - Part 2: 
    - Once deleting the previously forked repository, we will then refork the file to our github account. 
   
 - Part 3: 
    - This step doesn't have a real task but asks to start the timer to test how fast steps 4-9 could be done. 
 
 - Part 4: 
    - The real tasks begin now. From the terminal, we will first loggin to our ieng6 account.
    ![image](https://user-images.githubusercontent.com/122497278/221461456-148909d2-49d5-4734-a4d1-4672daa96e61.png)
    - From the terminal I used the ssh command followed by my user specific account (cs15lwi23aoi@ieng6.ucsd.edu) and then entered my password. 

 - Part 5: 
    - After logging into my ieng6 account, I went to my github acount to copy the ssh link of the repository that needed to be cloned. (git@github.com:justiiinnN/lab7.git). 
    ![image](https://user-images.githubusercontent.com/122497278/221472060-5e1d804d-2c8c-4f56-8e95-b6a5f3741870.png)
    - Using the command, ***git clone (Link)***, I was able to clone the repository. 

 - Part 6: 
    - Compiling and testing the file within the clone repository is the next step. 
    - The specific codes to compile and test is, ***javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java***, and ***java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore (file)***. 
    ![image](https://user-images.githubusercontent.com/122497278/221473382-25929d13-1acd-40e5-a78d-8983e5038b21.png)
    - This image shows that the file compiled but as an error. 
   
 - Part 7: 
    - It is time to fix the error within the code. This part is the most challenging! 
    - First, we must nano into the file to see the entirety of the code, ***nano (file)***. 
    ![image](https://user-images.githubusercontent.com/122497278/221474546-13c4010c-4a0b-4b15-ac90-e77bde7ed49a.png)
    - Doing nano props up the code in which the user could edit. Nano specifically is a terminal based file/text editor.  
    ![image](https://user-images.githubusercontent.com/122497278/221475016-6579e916-5eda-4af0-9ec0-ce604c745bad.png)
    - Since the code that has the error is in the ListExamples.java file, we nano to it in order to find and fix the flaw. 
    - The error was in one of the while loops. 
      - the wrong index was being added. 
    ```
    while(index2 < list2.size()){
     result.add(list2.get(index2)); 
     index1 += 1; 
    } 
    ```  
   - To fix the error, I had to change the index1 to index2. 
   - The revised code snippet: 
   
    ```
    while(index2 < list2.size()){
     result.add(list2.get(index2)); 
     index2 += 1; 
    } 
    ```  
   - After editing the code snippet I used the command, ***ctrl + o***. 
     - The ctrl + o command saves the edits made inside nano.  
     - Once saved, press and then `<enter>`
   
   
   
 - Part 8: 



up 6 to get junit after fixing code (javac) then presed enter
up 5 times to get junit (java) then pressed enter 
