# Optimized Sliding Window

## Overview
The **Sliding Window** technique is an efficient way to solve problems involving contiguous subarrays. Instead of recalculating sums from scratch, we use a window that slides across the array to maintain an optimized computation.

## Steps
1. Compute the sum of the **first `k` elements**.
2. Slide the window forward:
   - Add the **next element**.
   - Remove the **first element** from the previous window.
3. Update the maximum sum accordingly.

## Implementation (JavaScript)
```javascript
function maxSubarraySum(nums, k) {
  let maxSum = 0;
  let currentSum = 0;

  // First window sum
  for (let i = 0; i < k; i++) {
    currentSum += nums[i];
  }
  maxSum = currentSum;

  // Slide the window
  for (let i = k; i < nums.length; i++) {
    currentSum += nums[i] - nums[i - k]; // Add