# Lab report 4

## Links

* [My markdown-parse repo](https://github.com/tag717/markdown-parse)
* [Reviewed repo](https://github.com/vs2961/markdown-parse)

---
## Expected results

* ![snippet1expected](https://github.com/tag717/cse15l-lab-reports/blob/main/images4/Screen%20Shot%202022-02-25%20at%202.19.58%20PM.png?raw=true)
* Expected ```"`google.com", "google.com", "ucsd.edu"``` for snippet 1.
* ![snippet2expected](https://github.com/tag717/cse15l-lab-reports/blob/main/images4/Screen%20Shot%202022-02-25%20at%202.20.21%20PM.png?raw=true)
* Expected ```"a.com", "a.com(())"``` for snippet 2.
* ![snippet3expected](https://github.com/tag717/cse15l-lab-reports/blob/main/images4/Screen%20Shot%202022-02-25%20at%202.20.48%20PM.png?raw=true)
* Expected ```"https://ucsd-cse15l-w22.github.io/"``` for snippet 3.

---
## Tests

![tests I made](https://github.com/tag717/cse15l-lab-reports/blob/main/images4/Screen%20Shot%202022-02-25%20at%203.55.00%20PM.png?raw=true)

---
## Output for reviewed

![image](https://github.com/tag717/cse15l-lab-reports/blob/main/images4/Screen%20Shot%202022-02-25%20at%203.48.02%20PM.png?raw=true)
---
## Output for my repo

![image](https://github.com/tag717/cse15l-lab-reports/blob/main/images4/Screen%20Shot%202022-02-25%20at%203.46.26%20PM.png?raw=true)
![image](https://github.com/tag717/cse15l-lab-reports/blob/main/images4/Screen%20Shot%202022-02-25%20at%203.45.52%20PM.png?raw=true)
![image](https://github.com/tag717/cse15l-lab-reports/blob/main/images4/Screen%20Shot%202022-02-25%20at%203.46.07%20PM.png?raw=true)

---
## Questions
1. Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.
* We were only expecting ```"`google.com", "google.com"``` but ended up getting ```"url.com"``` as well. I believe we need less than 10 line code to fix this because we just need to check the backtik infront of the link and break.
2. Do you think there is a small (<10 lines) code change that will make your program work for snippet 2 and all related cases that nest parentheses, brackets, and escaped brackets? If yes, describe the code change. If not, describe why it would be a more involved change.
* I do think there is a small code change to fix this. We are getting the result back without ```))``` for ```"a.com(())"```. This is because we break when we see ```)```. 
Therefore, I think we just need to check for another ```)``` before breaking right away.
3. Do you think there is a small (<10 lines) code change that will make your program work for snippet 3 and all related cases that have newlines in brackets and parentheses? If yes, describe the code change. If not, describe why it would be a more involved change.
* I think for this we can change it would a small code change. I think we just have to see if there is a line break. However, currently I do not know the exact code to check the condition of line break.


