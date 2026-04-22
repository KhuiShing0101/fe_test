# 1 
Q1.In the single precision format of the “IEEE Standard for Binary Floating-Point Arithmetic”
(IEEE 754), a 32-bit floating point number is represented as below:
S: Sign (1 bit)
E: Exponent (8 bits)
F: Fraction (23 bits)
If 0 < E < 255, then the value of the number is (–1)S × 2 (E–127) × (1+F)
where F represents the fractional part of the number, stored as a 23-bit binary sequence. This
F is the sum of its weighted binary components: F=b1×2−1+b2×2−2+⋯+b23×2−23 , where b₁,
b₂, …, b₂₃ are the binary digits of F.
According to the IEEE-754 standard, which of the following is the decimal equivalent of the
32-bit floating point number given below?
01000001011000000000000000000000
a) 0.1875
b) 0.4375
c) 6.0
d) 14.0


#### 1. Split fields
- Sign (S) = `0` → positive  
- Exponent (E) = `10000010`  
- Fraction (F) = `11000000000000000000000`  

---

#### 2. Exponent calculation
Binary `10000010` = 130  

Exponent value:
E - 127 = 130 - 127 = 3  

---

#### 3. Fraction calculation
F = 1×2⁻¹ + 1×2⁻²  
  = 0.5 + 0.25  
  = 0.75  

So:
1 + F = 1.75  

---

#### 4. Final value
Value = (−1)ˢ × 2^(E−127) × (1 + F)  
      = (+1) × 2³ × 1.75  
      = 8 × 1.75  
      = 14.0  

---

### ✅ Answer:
**d) 14.0**

# 2
Q1.Let n be a binary integer represented in two’s complement. Which of the following is the
operation that results in the value 9 × n using only bit shifting and an addition or subtraction?
a) Shift n 2 bits to the left, then add n to the result.
b) Shift n 2 bits to the left, then subtract n from the result.
c) Shift n 3 bits to the left, then add n to the result.
d) Shift n 3 bits to the left, then subtract n from the result.

### explination
To compute \(9 \times n\) using bit shifts:

- Shifting left by 3 bits = \(n \times 2^3 = 8n\)

Now:
- \(8n + n = 9n\)

So the correct operation is:
**c) Shift n 3 bits to the left, then add n to the result.**

# 3
Q3.
Three friends and 4 other people are randomly seated in 7 seats arranged in a row. What is
the probability that the 3 friends sit next to one another?

)
1
168
b)
1
42
c)
1
35
d)
1
7

### Q3 Solution

Treat the 3 friends as a single block.

### Total arrangements:
7!  

### Favorable arrangements:
- Treat friends as one block → now we have 5 units (block + 4 others)
- Arrange these: 5! ways  
- Arrange friends within the block: 3! ways  

So:
Favorable = 5! × 3!

### Probability:
= (5! × 3!) / 7!  
= (120 × 6) / 5040  
= 720 / 5040  
= 1 / 7  

---

### ✅ Answer:
**d) 1/7**


# 4 