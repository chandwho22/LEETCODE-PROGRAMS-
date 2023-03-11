# LEETCODE-PROGRAMS-
Program Number 628
https://leetcode.com/problems/maximum-product-of-three-numbers/submissions/913393816/
import java.lang.Math;

class Solution {
    public int maximumProduct(int[] nums) {
        Arrays.sort(nums);//O(N)
        int n = nums.length;
        return Math.max(nums[n-1]*nums[n-2]*nums[n-3], nums[0]*nums[1]*nums[n-1]);
    }
}
