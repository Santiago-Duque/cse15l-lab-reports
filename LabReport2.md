## Lab Report 2 - `Code Changes`  
  
`Code Change #1:`  
![Code Change #1 CSE 15L Lab Report #2](https://user-images.githubusercontent.com/103283657/165244426-fd851016-f3e6-4f98-ad01-f263313eef67.png)  
[Link to the failure-inducing file](https://github.com/Santiago-Duque/cse15l-lab-reports/files/8608946/test-file2.md)  
  
Symptom: Wrong Answer Produced!  
  
![First Symptom CSE 15L Lab Report #2](https://user-images.githubusercontent.com/103283657/166419287-aa6a2b2e-2940-4cee-9d04-115edfd3375c.png)  
The first symptom was caused because everything to the right of the first bracket was detected, which produced the wrong output. The code change allowed code to the right of the first parenthesis to be detected, which produced the correct output.  
  
  
`Code Change #2:`  
![Second Code Change CSE 15L Lab Report #2](https://user-images.githubusercontent.com/103283657/166422098-9e2c12a0-5186-4090-9742-8e2ebe67e839.png)  
[Link to the failure-inducing file](https://github.com/Santiago-Duque/cse15l-lab-reports/files/8609099/test-file3.md)  
  
Symptom: An Infinite Loop!  
![Second Symptom CSE 15L Lab Report #2](https://user-images.githubusercontent.com/103283657/166421553-211a4f59-5d92-4824-834e-d28b8c15ce05.png)  
The toReturn arraylist would return an infinite loop because, in specific test cases where a closing bracket or parenthesis were not present, the code would infinitely run through each index. Therefore, this code ensures there's an open bracket or parenthesis through checking if it does NOT, resulting in the return of the toReturn arraylist.
  
`Code Change #3:`  
![Third Code Change CSE 15L Lab Report #2](https://user-images.githubusercontent.com/103283657/166423815-2132e2d9-ab71-4b51-8e39-d7c73c7aaddd.png)  
[Link to the failure-inducing file](https://github.com/Santiago-Duque/cse15l-lab-reports/files/8609196/test-file2.md)  
  
Symptom: Another Infinite Loop!  
![Third Symptom CSE 15L Lab Report #2](https://user-images.githubusercontent.com/103283657/166424116-597537a9-8e7e-41a6-abea-78459fab7f13.png)  
I tried changing the location in which the code would put an end to the infinite loop. After detecting the brackets and the parenthesis, the infinite loop was paused!

