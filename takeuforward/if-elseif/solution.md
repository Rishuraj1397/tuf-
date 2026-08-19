# If ElseIf

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/if-elseif
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    void studentGrade(int marks) {
        if(marks >= 90){
            cout << "Grade A";
        }else if (marks >= 70){
            cout << "Grade B";
        }else if (marks >= 50){
            cout << "Grade C";
        }else if (marks >= 35){
            cout << "Grade D";
        }else{
            cout << "Fail";
        }
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
