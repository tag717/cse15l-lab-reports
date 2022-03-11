# Lab Report 5

## Explain: how I found the tests with different results.
* I found the results by first getting the results from each repos. Next, I used ```diff``` command with the corrosponding folders and file names. Code: ```diff markdown-parse/output.txt MD-parse/markdown-parse/results.txt``` . From this output, I was able to easily compare the test results in both repo to analyze the differences. 
---
* The following two screen shots show the two tests results from the above command. 

![image](https://github.com/tag717/cse15l-lab-reports/blob/main/images5/Screen%20Shot%202022-03-11%20at%2011.43.14%20AM.png?raw=true)

![image](https://github.com/tag717/cse15l-lab-reports/blob/main/images5/Screen%20Shot%202022-03-11%20at%2011.43.20%20AM.png?raw=true)
* For test 194, the expected output was ```[url]``` according to the commonmark file. However, my repo resulted in nothing but the given code had the correct result. I think my repo markdownparse should have try to execute even with the under dash sign because I think it is breaking with the under dash sign ```_```. For this, I do not have the current code to fix. I just need to add a code that finds the under dash and try to ignore the part and continue to parse despite the under dash.
![image](https://github.com/tag717/cse15l-lab-reports/blob/main/images5/Screen%20Shot%202022-03-11%20at%2011.51.53%20AM.png?raw=true)
* For test 201, the expect output was ```[]``` as no links are shown in the preview of common mark. Therefore, for this test file, I believe that my repo's markdown-parse file was correct and the given one had the wrong result. I think to fix this, the code just need an addition of finding the ```<```. When I tested without ```<>``` the link appears for the expect output. So, I think when there is a ```<>``` it should break.
![image](https://github.com/tag717/cse15l-lab-reports/blob/main/images5/Screen%20Shot%202022-03-11%20at%2011.59.45%20AM.png?raw=true) 

* Code to change. For this first error, like I said above, we need to add a code that continues after the under dash. We could find the under dash and try to ignore and use ```continue```like the below code does to continue parsing.
For the second error, we should add a code to find the index of ```<>``` and try to break if it exists (find the index like the one below code).
![image](https://github.com/tag717/cse15l-lab-reports/blob/main/images5/Screen%20Shot%202022-03-11%20at%2012.23.29%20PM.png?raw=true) 
