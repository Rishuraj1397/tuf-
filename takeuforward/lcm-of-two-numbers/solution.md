# LCM of two numbers

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/lcm-of-two-numbers
- **Date:** 2026-07-26

## Solution

```cpp
// class Solution {
// public:
//     int LCM(int n1,int n2) {
//         int lcm;
        
//         int n = max(n1, n2);
//         int i = 1;
        
//         while(1) {
//             int mul = n * i;
            
//             if(mul % n1 == 0 && mul % n2 == 0) {
//                 lcm = mul;
//                 break;
//             }
//             i++;
//         }
        
//         return lcm;
//     }
// };

class Solution {
private:
    /* Function to find the
    GCD of two numbers*/
    int GCD(int n1, int n2) {
        
        /* Continue loop as long as both 
         n1 and n2 are greater than zero */
        while(n1 > 0 && n2 > 0) {
            
            /* If n1 is greater than n2, perform
             modulo operation - n1 % n2 */
            if(n1 > n2) {
                n1 = n1 % n2;
            }
            
            /* Else perform modulo
            operation - n2 % n1 */
            else {
                n2 = n2 % n1;
            }
        }
        
        // If n1 is zero, GCD is stored in n2
        if(n1 == 0) return n2;
        
        //else GCD is stored in n1
        return n1;
    }
    
public:
    // Function to find LCM of n1 and n2
    int LCM(int n1,int n2) {
        //Function call to find gcd
        int gcd = GCD(n1, n2);
        
        int lcm = (n1 * n2) / gcd;
        
        // Return the LCM
        return lcm;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
