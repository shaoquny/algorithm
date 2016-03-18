# algorithm
##Consolidate algorithm-learning

###1.快速排序 分治法
  * 选定一个元素作为中间值，将列表元素小于中间值的排左边，大于中间值的排右边
  * 将上述左边序列和右边序列分别用上述方式重复，一般以递归方式做。这就可以把一个长序列分成两个短序列分别处理，这就是分治法的核心思想。
  * 当短序列只剩下两个元素，就可以完全得出正确的序列，当序列小于两个元素可以直接忽略。


###2.0-1背包问题 动态规划（可得最优解），贪心（近似最优解）
  * 动态规划的核心思想也是把一个问题分成可以递推的子问题
  * 对于0-1背包，这边主要的算法思想是定义maxPrice(i, j)为经过前i个物品的抉择后背包被放了j体积的最大价值
  * 所以maxPrice(i, j) = max(maxPrice(i-1, j), maxPrice(i, j-v[i])+p[i])
 
 
###3.字符串子串匹配 kmp算法
  * 算法详解--> http://www.ruanyifeng.com/blog/2013/05/Knuth%E2%80%93Morris%E2%80%93Pratt_algorithm.html   
  * 本例中将匹配的字符串分成开始下标和结束下标存储在c++ pair类型中，因为可能有多条匹配，所以又将多个结果存储在vector中

