---
title: Binary Search Implementation
date: '2022-08-22'
tags: ['leetcode', 'algorithm', 'features']
draft: false
summary: Example of binary search Implementation
---

Test Post

```C++
int search(vector<int>& nums, int target) {
        int left = 0;
        int right = nums.size()-1;
        while(left <= right){
            int mid = left + (right - left)/2;
            if(nums[mid] < target){
                left++;
            } else if(nums[mid] > target){
                right--;
            } else{
                return mid;
            }
        }
        return -1;
    }
```