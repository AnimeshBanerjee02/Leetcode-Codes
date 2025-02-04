class Solution:
    def maxAscendingSum(self, nums: List[int]) -> int:
        prev = float("-inf")
        max_sum = curr = 0

        for num in nums:
            curr = curr+num if num > prev else num

            prev = num
            max_sum = max(max_sum, curr)

        return max_sum
