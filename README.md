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
