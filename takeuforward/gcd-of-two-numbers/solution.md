# GCD of Two Numbers

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/gcd-of-two-numbers
- **Date:** 2026-07-26

## Solution

```cpp
class Solution {
public:
    int GCD(int n1,int n2) {

        // brute force

        // int largest = 1;

        // for(int i = 2; i <= min(n1, n2); i++){
        //     if(n1 % i == 0 && n2 % i == 0){
        //         largest = i;
        //     }
        // }
        // return largest;


        // BETTER Approach

        // int largest;

        // for(int i = min(n1, n2); i >= 1; i--){
        //     if(n1 % i == 0 && n2 % i == 0){
        //         largest = i;
        //         break;
        //     }
        // }
        // return largest;


        // Optimal Approach
        while(n1 > 0 && n2 > 0){
            if(n1 > n2){
                n1 = n1 % n2;
            }else{
                n2 = n2 % n1;
            }
        }
        if(n1 == 0) return n2;

        return n1;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
