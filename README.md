# python-program
#powerofTwo
class Solution:
    def isPowerOfTwo(self, n: int) -> bool:
        if(n==0):
            return False
        else:
            return(n&(n-1))==0
ob=Solution()
n=1
print(ob.isPowerOfTwo(n))

#Subsets
class Solution:
    def subsets(self, nums: List[int]) -> List[List[int]]:    
        n=len(nums)
        total_subsets=1<<n
        ans=[]
        for num in range(total_subsets):
            temp=[]
            for i in range(n):
                if(num&(1<<i))!=0:
                    temp.append(nums[i])
            ans.append(temp)
        return ans
ob=Solution()
nums=[1,2,3]
print(ob.subsets(nums))
        
