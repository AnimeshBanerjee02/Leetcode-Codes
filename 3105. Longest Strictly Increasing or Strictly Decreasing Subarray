class Solution:
    def longestMonotonicSubarray(self, nums: List[int]) -> int:
        if len(nums) == 0:
            return 0
        if len(nums) == 1:
            return 1
        dec = 1
        inc = 1
        ans = 0
        for i in range(0,len(nums)-1):
            if nums[i]>nums[i+1]:
                dec+=1
                inc = 1
            elif nums[i]<nums[i+1]:
                inc+=1
                dec = 1
            else:
                inc = dec =1
            ans = max(ans,inc,dec)

        return ans
