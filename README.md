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