# Lab Report 2

## First issue
<img src="https://github.com/tag717/cse15l-lab-reports/blob/main/images/Screen%20Shot%202022-01-28%20at%203.46.51%20PM.png" width="400" height="400" />.
* First symptom was showing an infinite loop, which we did not wanted. When testing [lab.md](https://github.com/tag717/markdown-parse/blob/main/lab.md), 
nextOpenBracket wasn't being found and was assigned a value of -1. Therefore, we added a condition where if nextOpenBracket is equal to -1, we would break.
<img src="https://github.com/tag717/cse15l-lab-reports/blob/main/images/Screen%20Shot%202022-01-28%20at%203.43.00%20PM.png" width="600" height="300" />.

---
## Second issue
<img src="https://github.com/tag717/cse15l-lab-reports/blob/main/images/Screen%20Shot%202022-01-28%20at%203.08.58%20PM.png" width="800" height="100" />.
* Error with [labnew.md](https://github.com/tag717/markdown-parse/blob/main/labnew.md) file. This symptom was showing on our output. These lines should not be printing but it was getting printed. Therefore, we added a condition (line 17 and 18)
where it checks if the closed bracket is not right next to the open paranthesis,
if not it breaks.

<img src="https://github.com/tag717/cse15l-lab-reports/blob/main/images/Screen%20Shot%202022-01-28%20at%203.21.09%20PM.png" width="600" height="300" />.

---
## Third issue
<img src="https://github.com/tag717/cse15l-lab-reports/blob/main/images/Screen%20Shot%202022-01-28%20at%204.06.34%20PM.png" width="800" height="50" />.
* Error with [test-file6.md](https://github.com/tag717/markdown-parse/blob/main/test-file6.md) file. This file should not print [page.com] since it is an image with the ! sign. Therefore, we added a condition where if the '!' sign does not exist before the open paranthesis,
we print the statement inside the closed breackets.
<img src="https://github.com/tag717/cse15l-lab-reports/blob/main/images/Screen%20Shot%202022-01-28%20at%204.33.36%20PM.png" width="800" height="150" />.
