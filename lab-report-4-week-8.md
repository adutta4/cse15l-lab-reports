# Lab Report 4
## Markdown Parse Testing

[Link to my markdown-parse repository](https://github.com/adutta4/markdown-parse)  
[Link to reviewed markdown-parse repository](https://github.com/pvijay03/markdown-parse)

### Code Snippet 1
The expected outputs were checked with the [CommonMark website](https://spec.commonmark.org/dingus/): 

![s1-output](s1output.png)

The snippet was added to a file called snippet-1.md, and the added test is: 

![snippet1](snippet1.png)

The test failed for my implementation, with the following output: 

![s1fail](s1-fail.png)

The test failed for the implementation that my lab reviewed, with the following output: 

![s1-fail-review](s1-fail-r.png)

This code would likely be a more involved change. The code that you would need to add would have to check for the backticks, and make sure that the required parts of the links, such as the brackets in the first line of this snippet, are not within backticks (the reason why the first line is not rendered as a link). At the same time, the other examples below show that backticks are allowed within the brackets and in the link, and these are still rendered as links. As a result, you would need to check the locations of both backticks in relation to the parts of the link to determine whether it is a link or not. 

### Code Snippet 2
The expected output is: 



### Code Snippet 3
The expected output is: 


The snippet