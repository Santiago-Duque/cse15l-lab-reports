## Lab Report 2 - `Code Changes`  
  
`Code Change #1:`  
![Code Change #1 CSE 15L Lab Report #2](https://user-images.githubusercontent.com/103283657/165244426-fd851016-f3e6-4f98-ad01-f263313eef67.png)  
I edited the block of code (red is original, green is edited) because the following test:  
![Code Change #1 Broken Link CSE 15L Lab Report #2](https://user-images.githubusercontent.com/103283657/165246249-077cd135-1297-46d6-af93-60cf8a89b8be.png)  
resulted with the output being:  
![Code Change #1 Wrong Output CSE 15L Lab Report #2](https://user-images.githubusercontent.com/103283657/165245636-1f676151-58d8-4906-80a0-cd661e8d6dd2.png)  
instead of `[https://nothing.com, no-thing.html]`  
  
**THINGS TO NOTE:** Since the original code only detects for parentheses and brackets, the output expected was not received. Therefore, I had to comment out the lines of code involving brackets in order to solely detect parentheses. By detecting parentheses, the links for each item were detected and printed out as expected.  
