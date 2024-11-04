# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  Asymptotics drops constants and lower order terms because asymptotics is focused on growth rate. As n approachs infinity, lower order terms and exponents matter less, so when using asymptotics, we only need to care about the high order terms even though lower order terms have an impact on actual runtime with smaller values of n.
  
  Asymptotics only gives general bounds for runtimes, as asymptotics provides answers as n approachs infinity, meaning that could be a large difference in runtimes between two programs who both have the same asymptotic expression.

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

  The two datasets may have simply been run on different machines. The difference in hardware between the two machines is crucial to runtimes. The first machine could have had a faster processor, more memory, or less background programs which could all have made a program run faster than on a secondary machine which has a slower processor, less memory, and more background programs which all would greatly reduce the speed of the program.
  
  There could be various real-world issues like memory issues, CPU issues, or one of any number of bottlenecks or resource allocations in the machine that cause the program to run much slower. For example, a computer might be bottlenecked by using another program or function at the same time, which might limit access to memory, which might be impacting the larger 10,000 element tree more than the smaller 1,000 element tree as memory and resource needs increase.
  
  The optimization of a function may be an issue here. The complexity in part two and the given runtimes are calculated using assumed optimization and efficacy, but a poorly optimized or ineffective program will become slower. While this does apply to a smaller dataset, the effect is less noticeable, especially if we assume best-case scenario in the smaller tree, and a worst case in the larger tree. Worst cases would make the poorly optimized program even worse, leading to longer runtimes. If the code is ineffective and the smaller tree is not the worst case, the larger tree could exasperate problems found in the code and lead to the longer runtime. An example of this would be bad memory handling practices. Having to recall data repeatedly or creating multiple new trees or something like that could be part of the cause of the slowdown.
  
Add your answers to this markdown file.

I used this link to help with the misleading question: https://www.geeksforgeeks.org/asymptotic-notation-and-analysis-based-on-input-size-of-algorithms/ 
Got the complexity of the binary search tree from this link: https://testbook.com/maths/binary-search-tree#:~:text=In%20a%20balanced%20BST%2C%20the,and%20proceed%20left%20or%20right.

Worked with Michael Stoll to clean up my usage of terms. Talked to Lily Brongo about other options.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
