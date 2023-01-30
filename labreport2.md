# Lab Report 2 
---
### Part 1 
Provided below is the code snippet for the StringServer: 

<img width="932" alt="Screenshot 2023-01-30 at 3 09 35 PM" src="https://user-images.githubusercontent.com/122497278/215617434-b6ddc967-f573-4133-934c-607bc02875f4.png">

Two screenshots will be shown to demonstrate using /add-message. 
  - **The first screenshot**: 
  ![image](https://user-images.githubusercontent.com/122497278/215619228-d0d4338b-35cd-4300-9650-157fcb11e187.png)
    - The method being called in screenshot 1 is public String handleRequest.  
    - Relevant arguments to the method is the URI which in term is built of necessary characters that contains what is needed to find the method (StringServer) and ultimately the URL link (https://localhost:2100). StringServer is coded to display a string if the substring of **/add-message?s=** is inputed into the link (ex: https://localhost:2100/add-message?s=). To satisfy the codes requirement, a user must put in a word and or message (known as a string) after the equals sign in order to display that input. To exemplify, https://localhost:2100/add-message?s=hello displays the message "hello" on the website which is shown in the screenshot. Why this works is because after the s=, the code reads the users input as a string. 
    - Based on the request of the user made by inputting a string after the s=, the method checks the conditions and implements the paramters to show the user input. The empty string in place of paramter 2 is updated to what the user 

### Part 2 

### Part 3
In lab week 3, I would say that I learned quite alot. What I had learned was the basics of creating test cases that work to highlight the functionality of methods within code. Previously, I had no prior knowledge as to self testing code due to graders doing that for us students. After the lab, I applied my new knowledge to self test whenever I create code through creating my own hidden test cases and public tests cases all in which to sight bugs in code.

