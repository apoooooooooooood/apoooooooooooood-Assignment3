رابط الاكونت وجواه حل المساله 
https://leetcode.com/u/apderahmanezat2025/ 

حل مساله Solve LeetCode 136 — Single Number:
public class Solution
{
    public int FindSingleNumber(int[] nums)
    {
        int result = 0;

        foreach (int num in nums)
        {
            result ^= num;
        }

        // من الاخر لو الرقمين زي بعض الناتج صفر لو رقم مع صفر الناتج 1
        // so only the number appearing an odd number of times remains.
        return result;
    }
}