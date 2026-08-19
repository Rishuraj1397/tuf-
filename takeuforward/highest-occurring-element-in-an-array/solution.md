# Highest Occurring Element in an Array

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/highest-occurring-element-in-an-array
- **Date:** 2026-08-19

## Solution

```cpp
class Solution { //5 1 5 2 1 1
public:
    int mostFrequentElement(vector<int>& nums) {

        //Brute force
        // int n = nums.size();

        // int maxfreq = 0;

        // int maxEl = -1;

        // vector<bool> visisted(n,false);


        // for(int i = 0; i < n; i++){
        //     if(visisted[i]){
        //         continue;
        //     }

        //     int freq = 0;

        //     for(int j = i; j < n; j++){
        //         if(nums[i] == nums[j]){
        //             freq++;
        //             visisted[j] = true;
        //         }
        //     }


        //     if(freq > maxfreq){
        //         maxfreq = freq;
        //         maxEl = nums[i];
        //     }else if(freq == maxfreq){
        //         maxEl = min(maxEl, nums[i]);
        //     }
        // }
        // return maxEl;



        // Optimmal Solution

        int n = nums.size();

        int maxfreq = 0;

        int maxEl = -1;

        unordered_map<int, int> mpp;

        for(int i = 0; i < n; i++){
            mpp[nums[i]]++;
        }

        for(auto it : mpp){
            int ele = it.first;
            int freq = it.second;


            if(freq > maxfreq){
                maxfreq = freq;
                maxEl = ele;
            }else if(freq == maxfreq){
                maxEl = min(maxEl, ele);
            }
        }
        return maxEl;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
