---
layout: page
title: "About the Project"
permalink: /about/
---

The Function Graph Overview project is an open-source tool designed to help developers and students understand the flow of functions within their code. It visualizes how functions interact and connect, making it easier to analyze and debug programs.

For now the project supports several programming languages, including:
- C
- C++
- Python
- Go
- JavaScript and TypeScript (experimental)

By analyzing the input code, the tool generates a visual representation of the flow within a specific function. This includes identifying loops, conditions, and other structural elements, providing a detailed view of the function's behavior.

For example, here we can see a very simple C code from the demo platform:

```c
public void exampleFunction()
{
    int i;
    for (i = 0; i < 100; i++)
    {
        printf("Hello world\n");
    }
    if (i % 2 == 0)
    {
        printf("Yes!\n");
    }
    else
    {
        printf("No\n");
    }
}
```

The output graph generated for the user looks like this:

<img src="/assets/images/graphAbout.png" alt="Function Graph Example" style="max-width:400px; display:block; margin:2em auto;" />

The entry point is marked in green, and the exit point is in red.  
On the left section, the for loop is displayed, while the section on the right represents the code after the loop ends.  
The black block indicates the if statement, and the adjacent block on the right shows the else section.

Additionally, users can choose a "simplify" option to generate a less detailed graph. This mode abstracts basic commands while preserving key structural elements, providing a higher-level view of the function's flow:

<img src="/assets/images/graphAbout2.png" alt="Simplified Function Graph" style="max-width:400px; display:block; margin:2em auto;" />