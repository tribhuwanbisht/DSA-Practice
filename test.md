# DSA Practice

## Solution to Leetcode Problems using C++

### 1. Two Sum

![image](https://user-images.githubusercontent.com/91203793/232322540-bf2c8699-155d-4311-af71-75e8206b622d.png)
![image](https://user-images.githubusercontent.com/91203793/232322566-569d527d-530c-43bc-a540-efd733f10d09.png)

### Solution

```c++

class Solution {
    public int[] twoSum(int[] nums, int target) {
        int[] val = new int[2];
        for(int i=0;i<nums.length;i++)
        {
            for(int j=i+1;j<nums.length;j++)
            {
                if((nums[i] + nums[j]) == target)
                {
                    val[0] = i;
                    val[1] = j;
                }
            }
        }
        return val;
    }
}
```
