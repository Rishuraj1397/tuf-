# Second Highest Occurring Element

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/second-highest-occurring-element
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    int secondMostFrequentElement(vector<int>& nums) {


        // Brute force
        // -------------------------------------
        // int n = nums.size();
        // vector<bool> visited(n , false);

        // int maxfreq = 0;
        // int SecMaxFreq = 0;
        // int maxEl = -1;
        // int secMaxel = -1;


        // for(int i = 0; i < n; i++){

        //     if(visited[i]){
        //         continue;
        //     }

        //     int freq = 0;


        //     for(int j = i; j < n; j++){
        //         if(nums[i] == nums[j]){
        //             freq++;
        //             visited[j] = true;
        //         }
        //     }

        //     if(freq > maxfreq){
        //         SecMaxFreq = maxfreq;
        //         maxfreq = freq;
        //         secMaxel = maxEl;
        //         maxEl = nums[i];
        //     }else if(freq == maxfreq){
        //         maxEl = min(maxEl, nums[i]);
        //     }else if(freq > SecMaxFreq){
        //         SecMaxFreq = freq;
        //         secMaxel = nums[i];
        //     }else if(freq == SecMaxFreq){
        //         secMaxel = min(secMaxel, nums[i]);
        //     }
        // }
        // return secMaxel;




        // Optimized one
        // --------------------------------------------------
        int n = nums.size();
        int maxfreq = 0;
        int SecMaxFreq = 0;

        int maxEl = -1;
        int secMaxel = -1;

        unordered_map<int, int> mpp;

        for(int i = 0; i < n; i++){
            mpp[nums[i]]++;
        }


        for(auto it : mpp){
            int ele = it.first;
            int freq = it.second;



            if(freq > maxfreq){
                SecMaxFreq = maxfreq;
                maxfreq = freq;
                secMaxel = maxEl;
                maxEl = ele;
            }
            else if(freq == maxfreq){
                maxEl = min(maxEl, ele);
            }
            else if(freq > SecMaxFreq){
                SecMaxFreq = freq;
                secMaxel = ele;
            }
            else if(freq == SecMaxFreq){
                secMaxel = min(secMaxel, ele);
            }
        }

        return secMaxel;
        

        
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
