# Leetcode---1980
Find Unique Binary String
//code in java
class Solution {
    public String findDifferentBinaryString(String[] nums) {
        StringBuilder unique = new StringBuilder();
        int n = nums.length;
        
        for (int i = 0; i < n; i++) {
            // Flip the ith bit of the ith string
            unique.append(nums[i].charAt(i) == '0' ? '1' : '0');
        }
        
        return unique.toString();
    }
}
