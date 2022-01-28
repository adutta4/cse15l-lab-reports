# Lab Report 2
## Tests, Symptoms, and Bugs
### Code Change #1

![picture-fix](fix-pictures.png)
Test File: [Picture Output](https://github.com/adutta4/markdown-parse/blob/14dfb3ba8ee81a8bc85b25dfd5fc381120ea2139/testfile3.md)  
Symptom: 

In this case, the failure-inducing output is a markdown file that contains an image link only. The symptom is the output from running the getLinks method with this test file, and that it returns the image link, while the problem specifies that it should not do so. The bug here is that the code never makes a distinction between image links and website links. Since the structure is so similar, with only one character different, it adds the image link to the returned list in getLinks; the change in code is to make sure that there is no exclamation mark before the link.