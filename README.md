# Day 1 - Palindrome Number

🚀 Starting my #100DaysOfLeetCode challenge with #DSAwithedSlash

## Problem
Given an integer `x`, return `true` if `x` is a palindrome, and `false` otherwise.

---

# Problem Screenshot

![Problem Screenshot](Screenshot%202026-05-19%20140113(1).png)

---

# Java Solution

```java
class Solution {
    public boolean isPalindrome(int x) {

        if(x < 0){
            return false;
        }

        int n = x;
        int revNum = 0;

        while(n > 0){

            int d = n % 10;

            revNum = revNum * 10 + d;

            n = n / 10;
        }

        if(revNum == x){
            return true;
        }
        else{
            return false;
        }
    }
}
