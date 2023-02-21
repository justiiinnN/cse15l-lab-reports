# Lab Report 3 
--- 
The command that I will be choosing is *grep* and I will be demonstrating different ways of using it. 

 - Example 1: The first command that will be shown is, grep “ *[^number]” filename. Source used: [Link](https://www.softwaretestinghelp.com/grep-command-in-unix/)
   -  Input 1: 
 
     ```
    grep " *[3]" find-results.txt
    ``` 
    
   - Output 1: 
 
    ```
    written_2/non-fiction/OUP/Abernathy/ch3.txt
    written_2/non-fiction/OUP/Kauffman/ch3.txt
    written_2/non-fiction/OUP/Rybczynski/ch3.txt
    ``` 
   - Input 2: 
   ```
    grep " *[4]" find-results.txt
    ``` 
   - Output 2: 
 
    ```
    written_2/non-fiction/OUP/Abernathy/ch14.txt
    written_2/non-fiction/OUP/Berk/CH4.txt
    written_2/non-fiction/OUP/Kauffman/ch4.txt
    ``` 
     - grep “ *[^number]” filename, is useful if the user is trying to find specific files that have a certain number in it. 
 
 
 
 - Example 2: The second command that will be demonstrated is, *grep -i "string" filename*. Source used: [Link](https://qpeng.org/computer/grep.htm#:~:text=The%20%2Dc%20option%20tells%20grep,of%20%22boo%22%20in%20a_file.&text=An%20option%20more%20useful%20for,is%20%2Di%2C%20ignore%20case.)
      -  Input 1: 
 
     ```
    grep -i "CHI" find-results.txt
    ``` 
    
   - Output 1: 
 
    ```
    written_2/travel_guides/berlitz2/China-History.txt
    written_2/travel_guides/berlitz2/China-WhatToDo.txt
    written_2/travel_guides/berlitz2/China-WhereToGo.txt
    ``` 
   - Input 2: 
   ```
    grep -i "CU" find-results.txt
    ``` 
   - Output 2: 
 
    ```
    written_2/travel_guides/berlitz2/Cancun-History.txt
    written_2/travel_guides/berlitz2/Cancun-WhatToDo.txt
    written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt
    written_2/travel_guides/berlitz2/Cuba-History.txt
    written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt
    written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt
    ``` 
    - Unlike grep, *grep -i "string" filename* is good if the user is trying to find files that contain the string letters. The string can be taken in as a mix of lowercase and uppercase or all uppercase/lowercase. Grep itself will only find what is asked if the string doesnt have all uppercase letters. 
 
 
 
 - Example 3: The third command that will be shown is, *grep -c "string" filename*. Source used: [Link](https://qpeng.org/computer/grep.htm#:~:text=The%20%2Dc%20option%20tells%20grep,of%20%22boo%22%20in%20a_file.&text=An%20option%20more%20useful%20for,is%20%2Di%2C%20ignore%20case.)
      -  Input 1: 
 
     ```
    grep -c "China" find-results.txt
    ``` 
    
   - Output 1: 
 
    ```
    3
    ``` 
   - Input 2: 
   ```
    grep -c "France" find-results.txt
    ``` 
   - Output 2: 
 
    ```
    4
    ``` 
 
    - *Grep -c "string" filename*, is useful as it returns the number of how many files has the specified string. 
 
 
 - Example 4: The last command that will be demonstrated is, *grep -r "string" filename*. Source used: [Link](https://alvinalexander.com/linux-unix/recursive-grep-r-searching-egrep-find/)
   -  Input 1: 
 
     ```
    grep -r "Cu" find-results.txt
    ``` 
    
   - Output 1: 
 
    ```
    written_2/travel_guides/berlitz2/Cuba-History.txt
    written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt
    written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt
    ``` 
   - Input 2: 
   ```
    grep -r "Fr" find-results.txt
    ``` 
   - Output 2: 
 
    ```
    written_2/travel_guides/berlitz2/HistoryFrance.txt
    written_2/travel_guides/berlitz2/IntroFrance.txt
    written_2/travel_guides/berlitz2/WhatToFrance.txt
    written_2/travel_guides/berlitz2/WhereToFrance.txt
    ``` 
   - *grep -r "string" filename*, is useful when the user is trying to accomplish a recursive search with the goal of finding all the files in the directory with the users letter specific string input. 


