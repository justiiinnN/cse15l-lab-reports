# Lab Report 1
---
## Downloading VScode 
  * A link to the website where VScode can be downloaded is provided ([Link](https://code.visualstudio.com/))
    - From the link, VScode can be downloaded by clicking the big blue box that says "Download"
    <img width="1440" alt="Screen Shot 2023-01-14 at 11 59 05 PM" src="https://user-images.githubusercontent.com/122497278/212529444-4864f92c-8113-4821-8b31-cc571a4d3e67.png">
  * Downloading may take a few minutes or so depending on internet speed but once finished can be opened 
  * If download was successful, VScode will open up like so: 
  ![image](https://user-images.githubusercontent.com/122497278/212524074-d8a73805-a74c-4575-b780-b2ec86aa2517.png)

# Remotely Connecting 
 * Connecting to the server through VScode takes quite the steps 
    - To be able to connect to the class server we must have our CSE 15L account ready
    - Finding your CSE 15L account is simple and all it takes is going to the UCSD account lookup page [Link](https://sdacs.ucsd.edu/~icc/index.php)
    - The account lookup page looks like this: <img width="1440" alt="Screen Shot 2023-01-15 at 2 04 54 AM" src="https://user-images.githubusercontent.com/122497278/212534733-49b410e3-231c-4779-8899-ea8ff9d15b62.png">
 * Once the account details have been found and confirmed, open up VScode
 * Open up a new terminal within VScode where we will provide information to login into the server 
 * Within the terminal, put in your CSE15L username followed by @ieng6 and then .ucsd.edu 
    - As reference, what I would put into the terminal is **ssh cs15lwi23aoi@ieng6.ucsd.edu**
 * If you are prompted with "Are you sure you want to continue connecting (yes/no/[fingerprint])?", type yes and press enter
 * After typing yes, type in the password to your CSE15L account and if correct, you should be connected to the server! 

# Trying some commands 
 * Once in the sever, a variety of different commands are at the users disposal
 * Here are some examples of commands that can be used: 
   - cd
   - cd ~ 
   - ls -lat 
   - ls -a 
   - cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/
   - cat /home/linux/ieng6/cs15lwi23/public/hello.txt
  * Each command has its own use and purpose 
  * A command that I tested out was cd 
  <img width="1433" alt="Screen Shot 2023-01-11 at 4 07 45 PM" src="https://user-images.githubusercontent.com/122497278/212604537-3876df6d-5cd6-4282-9b37-aba2d98eead9.png">


