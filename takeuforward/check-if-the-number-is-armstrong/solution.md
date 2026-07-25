# Check if the Number is Armstrong

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/check-if-the-number-if-armstrong
- **Date:** 2026-07-25

## Solution

```cpp
class Solution {
private:
    /* Function to count the 
    number of digits in N */
    int countDigit(int n) {
        // Base case
        if(n == 0) return 1;
        int count = log10(n) + 1;
        return count;
    }
    
public:
    /* Function to find whether the
    number is Armstrong or not */
    bool isArmstrong(int n) {
        
        // Store the count of digits
        int count = countDigit(n);
        
        // Variable to store the sum, using long long to prevent overflow
        long long sum = 0;
        
        // Variable to store the copy
        int copy = n;
        
        /* Iterate through each
        digit of the number */
        while(n > 0){
            
            // Extract the last digit
            int lastDigit = n % 10;
            
            // Update sum
            sum += pow(lastDigit, count); 
            
            /* Remove the last digit
             from the number */
            n = n / 10;
        }
        
        /* Check if the sum of digits raised to the
        power of k equals the original number */
        if(sum == copy) return true;
        return false;
    }
};

```

---
*Generated automatically by LeetFeedback Extension*
