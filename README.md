## 3680. Generate Schedule
https://leetcode.com/problems/generate-schedule/description/
https://leetcode.com/problems/generate-schedule/solutions/7186393/easy-solution-keep-adding-teams/
if not res or ind1 not in res[-1] and ind2 not in res[-1] and tuple([ind1,ind2]) not in res_s:
not res: if res is empty, add pair to set.
ind1 not in res[-1] and ind2 not in res[-1]: check new pair does not have same as last pair
tuple([ind1,ind2]) not in res_s: check pair is not used b4.
for i in range(0, 2*(n+1)) is crucial. Changing it to n will create wrong ans for n=5. Changing it to 2*n will create wrong ans for n=6.
Greedy algorithm. O(N^2).
Tried to traverse matrix with loopback greedily results in wrong ans. Tried dfs results in TLE for n=6.

## 3690. Split and Merge Array Transformation
https://leetcode.com/problems/split-and-merge-array-transformation/description/
constraint 6. BFS. set to avoid revisiting.
Short code:
C++: https://leetcode.com/problems/split-and-merge-array-transformation/solutions/7210528/simple-bfs-explanation-with-added-video-explanation/
Python: https://leetcode.com/problems/split-and-merge-array-transformation/solutions/7209653/just-combination-of-bfs-and-permutations-brute-force/

## 3691. Maximum Total Subarray Value II
https://leetcode.com/problems/maximum-total-subarray-value-ii/description/
no RMQ: https://leetcode.com/problems/maximum-total-subarray-value-ii/solutions/7210224/divide-and-conquer-no-rmq/
RMQ: https://leetcode.com/problems/maximum-total-subarray-value-ii/solutions/7209652/solution-with-constraint-k-n-n-1-2/
Beat 100%: https://leetcode.com/problems/maximum-total-subarray-value-ii/solutions/7210456/beats-100-simple-solution-using-max-heap-and-sparse-table/
RMQ Sparse table: https://leetcode.com/problems/maximum-total-subarray-value-ii/solutions/7211061/rmq-sparse-table-heap-for-maximum/
SQRT decomp: https://leetcode.com/problems/maximum-total-subarray-value-ii/solutions/7213409/square-root-decomposition-solution/