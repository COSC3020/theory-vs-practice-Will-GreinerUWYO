# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  Asymptotics drops constants and lower order terms because asymptotics is focused on the big picture. As n gets larger and larger, lower order terms and exponents matter less, so when using asymptotics, we only need to care about the high order terms even though lower order terms have an impact on actual runtime with smaller values of n.
  Asymptotics only gives general bounds for runtimes, as asymptotics provides answers as n gets larger and larger, meaning that could be a large difference in runtimes between two programs who both have the same asymptotic expression
  Asymptotics considers only the theoretical runtimes of the algorithm in a ideal system without taking into account external factors. Memory issues, computational issues, factors intrinsic to the programming, or a machine which cannot handle the code would perform worse than the asymptotic expression would suggest.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  Since a binary search tree has a complexity of O(log(n)), so finding an element in a tree with 1,000 elements takes 5 seconds, or 1.6 * log(1000) = 5 seconds.
   Which would mean that finding an element in a binary search tree with 10,0000 elements would take 1.6 * log(10,000) = 6.4 seconds.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

  The constants used for calculation that are dropped for complexity still have an effect, one which is more noticeable on larger datasets.
  There could be various real-world issues like memory issues, CPU issues, or one of any number of bottlenecks or resource allocations in the machine that cause the program to run much slower. For example, a computer might be bottlenecked by using another program or function at the same time, which might limit access to memory, which might be impacting the larger 10,000 element tree more than the smaller 1,000 element tree as memory and resource needs increase.
  The O(log(n)) complexity assumes a balanced tree. If the tree is unbalanced, it could be as bad as O(n), which would account some of the increased time, but not enough on its own, this issue would be compounded by the other reasons above.
  
Add your answers to this markdown file.

I used this link to help with the misleading question: https://www.geeksforgeeks.org/asymptotic-notation-and-analysis-based-on-input-size-of-algorithms/ 
Got the complexity of the binary search tree from this link: https://testbook.com/maths/binary-search-tree#:~:text=In%20a%20balanced%20BST%2C%20the,and%20proceed%20left%20or%20right.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
