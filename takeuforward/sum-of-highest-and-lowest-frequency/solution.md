# Sum of Highest and Lowest Frequency

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/sum-of-highest-and-lowest-frequency
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    int sumHighestAndLowestFrequency(vector<int> &nums) {
        
        int n = nums.size();
        
        int maxFreq = 0, minFreq = n; 
        
        unordered_map<int, int> mpp;
        
        for (int i = 0; i < n; i++) {
            mpp[nums[i]]++;
        }
            
        for(auto it : mpp) {
            int freq = it.second;
            
            maxFreq = max(maxFreq, freq);
            minFreq = min(minFreq, freq);
            
        }
        
        return maxFreq + minFreq;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
