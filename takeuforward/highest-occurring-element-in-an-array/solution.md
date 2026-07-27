# Highest Occurring Element in an Array

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/highest-occurring-element-in-an-array
- **Date:** 2026-07-27

## Solution

```cpp
class Solution {
public:
    /* Function to get the highest 
    occuring element in array n */
    int mostFrequentElement(vector<int> &nums) {
        
        // Variable to store the size of array
        int n = nums.size();
        
        // Variable to store maximum frequency
        int maxFreq = 0; 
        
        /* Variable to store element 
        with maximum frequency */
        int maxEle;
        
        // HashMap
        unordered_map<int, int> mpp;
        
        // Iterating on the array
        for (int i = 0; i < n; i++) {
            // Updating hashmap 
            mpp[nums[i]]++;
        }
            
        // Iterate on the map
        for(auto it : mpp) {
            int ele = it.first; // Key
            int freq = it.second; // Value
            
            if(freq > maxFreq) {
                maxFreq = freq;
                maxEle = ele;
            }
            else if(freq == maxFreq) {
                maxEle = min(maxEle, ele);
            }
        }
        
        // Return the result
        return maxEle;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
