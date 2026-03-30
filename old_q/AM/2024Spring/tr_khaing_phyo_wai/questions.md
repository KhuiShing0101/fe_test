Q5
DFS → explore deep paths first
BFS → explore wide/level first

1. Depth-First Traversals (DFS)
    Traversals 
    1.Inorder Traversals(Left → Root → Right)
            Used often in Binary Search Trees to get sorted order.

                20
             /    \
           10      30
          /  \    /  \
         5   15  25   40
        / \    \       \
       3   7    17      50
          / \           /
         6   8         45

        3, 5, 6, 7, 8, 10, 15, 17, 20, 25, 30, 40, 45, 50

    2.Preorder Traversals(Root → Left → Right)
        Useful for copying trees or prefix expressions.

               20
             /    \
           10      30
          /  \    /  \
         5   15  25   40
        / \    \       \
       3   7    17      50
          / \           /
         6   8         45

        20, 10, 5, 3, 7, 6, 8, 15, 17, 30, 25, 40, 50, 45

    3.Postorder (Left → Right → Root)
        Useful for deleting trees or postfix expressions.
               20
             /    \
           10      30
          /  \    /  \
         5   15  25   40
        / \    \       \
       3   7    17      50
          / \           /
         6   8         45

        3,6,8,7,5,17,15,10,20,25,45,50,40,30,20

2. Breadth-First Traversal (BFS)
    Level Order Traversal
               20
             /    \
           10      30
          /  \    /  \
         5   15  25   40
        / \    \       \
       3   7    17      50
          / \           /
         6   8         45

         20, 10, 30, 5, 15, 25, 40, 3, 7, 17, 50, 6, 8, 45

Yes, your traversal orders are correct:

In-order: left → root → right
Post-order: left → right → root
Pre-order: root → left → right

In e-commerce, tree traversals are often used for:

Category hierarchies – e.g., displaying categories and subcategories.
Inventory management – e.g., updating stock from leaf items to parent categories (post-order).
Recommendation engines – traversing user behavior trees for suggestions.

Basically, hierarchical data is the main use case.

Here’s a simple Markdown diagram showing tree traversals and e-commerce use cases:

# Tree Traversals in E-commerce

Consider a category tree:
      Electronics
     /          \
 Phones         Laptops
/     \        /      \
iPhone Samsung MacBook Dell

| Traversal Type | Order Visited                                                      | E-commerce Use Case                         |
|----------------|--------------------------------------------------------------------|---------------------------------------------|
| **Pre-order**  | Electronics → Phones → iPhone → Samsung → Laptops → MacBook → Dell | Display categories top-down (root first) |
| **In-order**   | iPhone → Phones → Samsung → Electronics → MacBook → Laptops → Dell | Sorted product listing in a category     |
| **Post-order** | iPhone → Samsung → Phones → MacBook → Dell → Laptops → Electronics | Update stock or aggregate data from leaves up |


✅ Summary:

Pre-order: Top-down view (like menus).
In-order: Sorted listings.
Post-order: Bottom-up calculations (e.g., total stock).

If you want, I can also make a tiny visual diagram showing arrows for each traversal so it’s super easy to memorize. Do you want me to do that?

-------------------------------------------------------------------------------------------------------------------------------------------------------------
Q6
-------------------------------------------------------------------------------------------------------------------------------------------------------------
The flowchart below shows an algorithm that determines the sum (i.e. “1 +3+ 5+ … +(2N-1)”) of the first N odd integers from 1 through 2N-1 (where N ≥ 1) and inserts the result into variable x. Which of the following is an expression to be inserted in blank A ? 


N = odd int
N odd integers
2N01 ( where N>/ 1 )
x= the final result
A = ?


-------------------------------------------------------------------------------------------------------------------------------------------------------------
Q7
-------------------------------------------------------------------------------------------------------------------------------------------------------------
How many swaps are required in bubble sort when N elements in the array are already sorted in reverse order?
a) N(N-1) ÷ 2 b) N 2 ÷ 2 c) N(N-1) d) N 2

## Bubble Sort (Worst Case)

Array: `[4, 3, 2, 1]` (reverse sorted)

- Total swaps = 6  
- Formula:  

N(N - 1) / 2


### Example:

3 + 2 + 1 = 6


### Key Points:
- Reverse order = worst case  
- Swaps = max = N(N-1)/2  
- Swaps ≠ passes (loops)


    ## Bubble Sort Cases

        ### 1. Best Case
        - Array already sorted → `[1,2,3,4]`
        - Swaps = 0  
        - Time = O(N)

        ---

        ### 2. Average Case
        - Random order → `[3,1,4,2]`
        - Swaps = medium  
        - Time = O(N²)

        ---

        ### 3. Worst Case
        - Reverse sorted → `[4,3,2,1]`
        - Swaps = N(N-1)/2  
        - Time = O(N²)

        Easy memory trick

        Best → already sorted → no swaps
        Worst → reverse → max swaps
        Average → in between

-------------------------------------------------------------------------------------------------------------------------------------------------------------
Q11
Which of the following is the design for securing safety and reliability known as “foolproof”? 
-------------------------------------------------------------------------------------------------------------------------------------------------------------

## Safety & Reliability Terms (Simple)

### 🔹 Foolproof
- Prevents mistakes
- User cannot do it wrong

### 🔹 Fail-safe
- If system fails → becomes safe
- Stops but safe

### 🔹 Fault-tolerant
- If system fails → keeps working
- Uses backup

### 🔹 Robust
- Handles errors or bad input
- Does not crash

---

## 🎯 Quick Trick

- Foolproof → no mistake allowed  
- Fail-safe → safe if fails  
- Fault-tolerant → still works if fails  
- Robust → handles errors  

## on software
Term	        Level
Foolproof	UI / input design
Fail-safe	System safety design
Fault-tolerant	System architecture
Robust	Code + system behavior

Easy way to remember
Architecture → fault-tolerant, fail-safe
Code/UI → robust, foolproof

-------------------------------------------------------------------------------------------------------------------------------------------------------------
Q15. Which of the following is the appropriate explanation of ideal hashing used during a data search?
-------------------------------------------------------------------------------------------------------------------------------------------------------------
