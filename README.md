# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.

Bullet 1

1. Asymptotic analysis is theoretical, as it describes algorithm behavior as the input reaches infinity.  Actual performance is empirical, as it describes algorithm behavior with a specific set of inputs.  

2. Actual performance is affected by hardware, software, and the characteristics of the input data, whereas asymptotic analysis is primarily affected by the input size.

3. Asymptotic analysis takes into account inputs reaching infinity.  This can be misleading, as it doesn’t consider small inputs, so the results of those inputs may not be accurately presented.

Bullet 2

The time complexity depends on if the binary search tree is balanced or not.  If it is balanced, it has a best case of O(1) and an average and worst case of O(log(n)).  If it isn’t balanced, it has a best case of O(1), and an average and worst case of O(n).

For a balanced binary tree, finding the same element in a tree of 10,000 elements takes about 6.65 seconds in the worst case, which comes from multiplying 5 by log2(10,000)/log2(1,000).  For an unbalanced binary tree, finding the same element in a tree of 10,000 elements takes about 50 seconds in the worst case, which comes from multiplying 5 by 10,000/1,000. 

Bullet 3

1. It could have taken much longer because the tree was very unbalanced, meaning the algorithm has to go through most, if not all of the nodes.  This causes a large difference because as mentioned above, if the tree is balanced it takes roughly 6.65 seconds, whereas when it is unbalanced it can take roughly 50 seconds.

2. The hardware specifications, such as CPU speed and memory size, have an affect on actual performance, no matter what input size, so it is possible that during the runtime the computer was doing many other tasks in the background, causing the time to take considerably longer than expected.

3. The software environment, such as the operating system and the compiler, have an effect on actual performance, no matter what input size.  If used on a different operating system or if a different compiler was used, the time could be shortened.


I received help from ChatGPT on 1.3 and 2.  For 1.3, I asked ChatGPT the question listed in the assignment.  Regarding 2, ChatGPT gave me the number of seconds it can take to find an element in a balanced binary tree of 10,000 elements.
