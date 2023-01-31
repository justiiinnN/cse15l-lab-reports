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
    - Based on the request of the user made by inputting a string after the s=, the method checks the conditions and implements the paramters to show the user input. The first parameter checks if there is an "s" and if there is the second parameter continues. The second parameter is the user's input string.
    The created empty string is added to paramter 2 and is updated to what the user had intended. 
  - **The second screenshot**: 
  ![image](https://user-images.githubusercontent.com/122497278/215653412-66c9f998-368d-4f2f-af5b-07571e45cc54.png)
    - The method being called in screenshot 2 is public String handleRequest
    - Relevant arguments to the method is identical to that of screenshot 1. If the user inputs another string after inputting one already, the method will take in the new string and display the first and latest input(s). 
    - Each time a new requests by the user is made, the code updates the page based on the string input. The first screenshot demonstrates the first user input of "hello" and the second shows the latest input of "world". Both inputs are displayed on the page as requests continue to be made. 

### Part 2 
  - The file ArrayExamples.java had different bugs that were to be tested and fixed
    - One of the bugs were in static int[]reversed(int[] arr):  
    
    ```
    static int[] reversed(int[] arr){
        int[] newArray = new int[arr.length]; 
        for(int i = 0; i < arr.length; i += 1){
          arr[i] = newArray[arr.length - i - 1]; 
         }
        return arr; 
       }
   - The method static int[]reversed(int[] arr), is supposed to return an array with all the elements reversed. If testing with Junit, the method does not pass all the test cases. 
   - A failure inducing input is shown below: 
   
    @Test 
    public void reverseInPlace(){
      int[] input1 = { 0, 1, 2, 3 }; 
      ArrayExamples.reverseInPlace(input1); 
      assertArrayEquals(new int[] { 3, 2, 1, 0 }, input1); 
     }
    }
   - An input that wouldn't induce a failure is an empty array, why this would pass is because there is nothing in the array to rearrange so the code would run fine with no errors. 
   
    @Test 
    public void reverseInPlace(){
      int[] input1 = {}; 
      ArrayExamples.reverseInPlace(input1); 
      assertArrayEquals(new int[] {}, input1); 
     }
    }
   - 
### Part 3
In lab week 3, I would say that I learned quite alot. What I had learned was the basics of creating test cases that work to highlight the functionality of methods within code. Previously, I had no prior knowledge as to self testing code due to graders doing that for us students. After the lab, I applied my new knowledge to self test whenever I create code through creating my own hidden test cases and public tests cases all in which to sight bugs within code.

