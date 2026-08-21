# Rotate String

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/rotate-string
- **Date:** 2026-08-21

## Solution

```cpp
class Solution{	
	public:
		bool rotateString(string& s,string& goal){
			// //your code goes here

            // // --------------Brute force-----------------

            // // If the size of both the string and goal is mismatched we will return false
            // if(s.size() != goal.size()){
            //     return false;
            // }


            // // Size of string 
            // int n = s.size();


            // //Trying every possible rotation
            // for(int i = 0; i < n; i++){
            //     //checking if current rotation matches the goal or not
            //     if(s == goal){
            //         return true;
            //     }


            //     //stores the first character
            //     char first = s[0];

            //     // Remove the first character
            //     s.erase(s.begin());

            //     // Move it to the end
            //     s.push_back(first);
            // }
            // return false;






            // ----------------Optimal soln-----------


            // checking the size of both the string 
            if(s.size() != goal.size()){
                return false;
            }

            string doubled = s + s;

            return doubled.find(goal) != string::npos;
            
		}
};
```

---
*Generated automatically by LeetFeedback Extension*
