# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  Asymptotics generally drops things like constants, as can be seen in the previous Divide and Conquer Sum answer for complexity.
  Asymptotics gives broad general answers for runtime questions, but doesn't accurately portray exact times, only giving general ranges. As runtime is not the same as complexity.
  Asymptotics considers only the theoretical runtimes of the algorithm on an empty and perfect machine, not taking into account other running programs or hardware differences.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  Since a binary search tree has a worst-case complexity of O(n), then finding the same element in a search tree with ten times as many elements should be a constant ten bigger, making the time to coomplete the 10,000 element search 50 seconds.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

  This program could have been run while the machine was running different programs, leading to a massive slowdown and causing the program to take far longer than expected to complete.
  The constants used for calculation that are dropped for complexity may have a larger effect on larger sets of numbers, leading to a longer runtime.
  The program could be a less efficient version of the code expected, leading to increases in runtime that get exasperated with larger datasets.
  
Add your answers to this markdown file.

I used this link to help with the misleading question: https://www.geeksforgeeks.org/asymptotic-notation-and-analysis-based-on-input-size-of-algorithms/ 
Got the complexity of the binary search tree from this link: https://www.geeksforgeeks.org/complexity-different-operations-binary-tree-binary-search-tree-avl-tree/

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
