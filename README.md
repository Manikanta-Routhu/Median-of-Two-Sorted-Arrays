# Median of Two Sorted Arrays

# Problem Description
Given two sorted arrays `nums1` and `nums2` of size `m` and `n` respectively, return the **median** of the two sorted arrays.

The overall run time complexity should be **O(log (m + n))**.

---

## 🧠 Example

**Input:**
```python
nums1 = [1, 3]
nums2 = [2]

output:
2.0

Explanation:
Merged array = [1, 2, 3]
Median = 2.0


Constraints

nums1.length == m

nums2.length == n

0 <= m <= 1000

0 <= n <= 1000

1 <= m + n <= 2000

-10^6 <= nums1[i], nums2[i] <= 10^6

Approach:

The goal is to achieve O(log(min(m, n))) time complexity using binary search.

We partition both arrays such that:

Left half and right half contain equal number of elements.

All elements in the left half are ≤ all elements in the right half.

Then:

If total length is odd → median = max(left half)

If even → median = average of max(left half) and min(right half)

Complexity Analysis:

| Type      | Complexity        |
| --------- | ----------------- |
| **Time**  | O(log(min(m, n))) |
| **Space** | O(1)              |

Example runs:

| nums1 | nums2 | Output |
| ----- | ----- | ------ |
| [1,3] | [2]   | 2.0    |
| [1,2] | [3,4] | 2.5    |
| [0,0] | [0,0] | 0.0    |
| []    | [1]   | 1.0    |

How to Run:

# Clone this repository
git clone https://github.com/YOUR_USERNAME/Median-of-Two-Sorted-Arrays.git

# Navigate into it
cd Median-of-Two-Sorted-Arrays

# Run the program
python median_two_sorted_arrays.py



