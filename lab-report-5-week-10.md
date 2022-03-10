# Lab Report 5
## Testing Markdown Parse

In order to find tests that had different results between my implementation and the provided implementation, I first ran both implementations separately. I then used `diff` on the resulting files to find tests that gave different outputs between both implementations. The output from `diff` indicates the line numbers that the differences occur on, and what the exact output of each implementation is, as shown below: 

![diff-run](diff-run.png)

### Test 1
The first test that I identified is 201.md, which contains the text:

![first](test-1.png)

The output from running `diff` for this test is shown below, where the results from my implementation are at the top, and the results from the provided implementation are at the bottom: 

![output1](1-out.png)

Using [CommonMark](https://spec.commonmark.org/dingus/), the expected output should have no links, meaning that my implementation is correct. For the provided implementation, the bug seems to be that there is no check for whether the open parentheses is located right after the closed bracket or not, so it finds the next open parentheses regardless of what is in between and considers it a link. In the code below, the code to address this should be added around line 65. 

### Test 2
The second test I identified was 