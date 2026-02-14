# Codeforces 1805A — We Need the Zero

🔗 Problem Link: https://codeforces.com/problemset/problem/1805/A

## Problem

Given an array `a`, find an integer `x` such that after replacing every element with:

the XOR of all elements in the new array becomes `0`.

If no such value exists, print `-1`.

---

## Approach




### Case 1: n is even
- All `x` values cancel out.
- Result = `S`
- Possible only if `S == 0`.

### Case 2: n is odd
- One `x` remains.
- `S ⊕ x = 0`
- Therefore, `x = S`.

---

## Algorithm

1. Compute XOR of all elements.
2. If `n` is odd → answer = total XOR.
3. If `n` is even:
   - if total XOR is `0` → answer = `0`
   - else → answer = `-1`.

---

## Complexity

- Time: `O(n)`
- Space: `O(1)`

---

## Key Idea

The solution depends only on how many times `x` appears in XOR:

- Even times → cancels out  
- Odd times → remains once
