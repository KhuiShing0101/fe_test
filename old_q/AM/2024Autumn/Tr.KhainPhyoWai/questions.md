# 1. Q5 ( Tree Diagram ) 
Algo What is the value of the arithmetic expression resulting from an in-order traversal of the binary tree below? 
            (/)
           /   \
         (-)    2
        /   \
      (*)    10
     /   \
   (+)    10
  /   \
 2     3
 a) 11 b) 20 c) 27 d) 45 

# 2. Q6. Method Recursive
The function f (n) is recursively defined in terms of the natural number n as below. Which
of the following is the value of f (5)?
f (n): if n≦1 then return 1 else return n + f (n−1) 
a) 6 b) 9 c) 15 d) 25 

# 3. Q7 Sort Algo
.Which of the following is the appropriate description of the “selection sort” algorithm?
a) An intermediate reference value is determined, and then the elements are divided into
two groups of “larger” values and “smaller” values. This operation is recursively
repeated.
b) Each set of elements extracted at regular intervals is sorted, and then the interval is
further decreased. The operation is repeatedly performed until the interval becomes 1.
c) The element with the largest value is determined and swapped for the last element, and
then the largest value of the unsorted elements is determined and swapped for the
second-to-the-last element. This operation is repeated in the same way.
d) Two adjacent elements are repeatedly compared and swapped if the first element is
larger than the second. This operation is repeated until all elements are arranged in an
orderly fashion
Sorting Algo

## bubble sort is left to right comparing adjcents
## selection sort is smallest to first pick and move on
## quick sort seperate 2 parts smaller and larger sort ( recursively make )

## Easy Memory Trick 🧠
“BIS” → Basic: Bubble, Insertion, Selection
“QMH” → Fast: Quick, Merge, Heap
“CRB” → Special: Counting, Radix, Bucket

## | Algorithm      | Best Time   | Avg Time   | Worst Time | Space    | Stable | Notes                        |
| -------------- | ----------- | ---------- | ---------- | -------- | ------ | ---------------------------- |
| Bubble Sort    | O(n)        | O(n²)      | O(n²)      | O(1)     | ✅ Yes  | Very simple, very slow       |
| Selection Sort | O(n²)       | O(n²)      | O(n²)      | O(1)     | ❌ No   | Few swaps                    |
| Insertion Sort | O(n)        | O(n²)      | O(n²)      | O(1)     | ✅ Yes  | Good for small/nearly sorted |
| Merge Sort     | O(n log n)  | O(n log n) | O(n log n) | O(n)     | ✅ Yes  | Stable, uses extra memory    |
| Quick Sort     | O(n log n)  | O(n log n) | O(n²)      | O(log n) | ❌ No   | Fastest in practice          |
| Heap Sort      | O(n log n)  | O(n log n) | O(n log n) | O(1)     | ❌ No   | No extra space               |
| Counting Sort  | O(n + k)    | O(n + k)   | O(n + k)   | O(k)     | ✅ Yes  | Only for small integer range |
| Radix Sort     | O(nk)       | O(nk)      | O(nk)      | O(n + k) | ✅ Yes  | Digit-based sorting          |
| Bucket Sort    | O(n)        | O(n + k)   | O(n²)      | O(n)     | ✅ Yes  | Works best for uniform data  |
| Shell Sort     | ~O(n log n) | ~O(n^1.5)  | O(n²)      | O(1)     | ❌ No   | Gap-based insertion          |
| Tim Sort       | O(n)        | O(n log n) | O(n log n) | O(n)     | ✅ Yes  | Used in Python/Java          |

bubble sort 
<?php 
fuction bubbleSort($arr){
    $n = count($arr);
    for($i=0;$i<$n-1;$j++){
        if($arr[$j])
    }
}
?>

# 4. Q8 What is the approximate performance of a CPU in MIPS, when the instruction mix of the CPU is shown in the table below? Here, the CPU does not use a pipeline architecture.

| Instruction Type                | Instruction Execution Time (µs) | Appearance Ratio |
|--------------------------------|--------------------------------|------------------|
| Register to register operation | 0.3                            | 30%              |
| Register to memory operation   | 0.6                            | 50%              |
| Conditional branch operation   | 0.1                            | 20%              |
a) 0.03 b) 0.41 c) 2.44 d) 35.00 

# 5. Q11.System design 
Which of the following is a fail-safe concept for improving the security and reliability
of the information system?


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



# 6. Q12.👉 “These are AND/OR reliability network questions”
 Which of the following is the approximate availability of the system comprising five devices, namely, A, B, C, D, and E as shown in the figure below? The numeric value in parentheses represents the availability of each device. The system is operational if either device connected in parallel is available. 

# 7. Q27.Phishing email
Q27. Which of the following is an example of a phishing email?
a) An email containing pop-up ads for products unrelated to the email
b) An email intercepted, altered, and successfully sent
c) An email with a link that automatically installs an application collecting and sending
data to the remote server
d) An email with a link that redirects to a fake banking site
## pretend to be finalcial or banking email is like phishing email

# 8. Q28.Computer Security  
Which of the following bitwise logical operation can be applied in stream cipher
between a plain text and a keystream to produce a cipher text, and between a ciphertext and
the keystream to recover the plaintext?
a) AND b) NAND c) OR d) XOR

## Bitwise Logical Operations (Short Notes)

### 1. OR
- Symbol: `|`
- Rule: Result is **1 if at least one bit is 1**

| A | B | A OR B |
|---|---|--------|
| 0 | 0 |   0    |
| 0 | 1 |   1    |
| 1 | 0 |   1    |
| 1 | 1 |   1    |

👉 Used to **set bits**

---

### 2. NOR
- Symbol: NOT OR
- Rule: Result is **1 only if both bits are 0**

| A | B | A NOR B |
|---|---|---------|
| 0 | 0 |   1     |
| 0 | 1 |   0     |
| 1 | 0 |   0     |
| 1 | 1 |   0     |

👉 Opposite of OR

---

### 3. NAND
- Symbol: NOT AND
- Rule: Result is **0 only if both bits are 1**

| A | B | A NAND B |
|---|---|----------|
| 0 | 0 |   1      |
| 0 | 1 |   1      |
| 1 | 0 |   1      |
| 1 | 1 |   0      |

👉 Opposite of AND  
👉 Important in digital circuits

---

### 4. XOR (Exclusive OR)
- Symbol: `^` or `⊕`
- Rule: Result is **1 if bits are different**

| A | B | A XOR B |
|---|---|---------|
| 0 | 0 |   0     |
| 0 | 1 |   1     |
| 1 | 0 |   1     |
| 1 | 1 |   0     |

👉 Used in **stream ciphers (encryption)**  
👉 Property: `A ⊕ B ⊕ B = A` (can reverse)

---

### 🧠 Quick Memory Tips
- OR → at least one 1  
- NOR → only 00 gives 1  
- NAND → only 11 gives 0  
- XOR → different = 1

# 9. Q29.Encryption 
Which of the following description is an appropriate use of asymmetric encryption to ensure the confidentiality of a message that a sender is going to send to a receiver?
a) The message is encrypted using a pre-shared secret key.
b) The message is encrypted using a private key of the sender.
c) The message is encrypted using a public key of the receiver.
d) The message is encrypted using a public key of the sender.

# 10 Q30.Attack 
Which type of attack involves intercepting communication between sender and receiver?
a) Brute Force Attack b) Man-in-the-Middle Attack
c) Phishing Attack d) Ransomware Attack 

a) Brute Force Attack → Trying many password/key combinations until the correct one is found.
b) Man-in-the-Middle Attack → Attacker secretly intercepts and possibly alters communication between sender and receiver. ✅
c) Phishing Attack → Tricking users into revealing sensitive info (like passwords) via fake emails/websites.
d) Ransomware Attack → Malware that locks/encrypts your data and demands payment to restore access.
## Here’s how to quickly “catch the point” in each option:

a) mentions dictionary words + one target user → trying word list ⇒ Dictionary attack
b) mentions leaked usernames/passwords from other websites ⇒ reuse of credentials ⇒ Credential stuffing
c) mentions one common password used across many user IDs ⇒ one password, many accounts ⇒ Password spraying
d) mentions all possible combinations of characters ⇒ trying everything ⇒ Brute force

### Simple trick:

Dictionary = word list
Stuffing = stolen real passwords
Spraying = one common password across many users
Brute force = try everything


# 11 Q31.Attack
 Q32. Which of the following is the name of an attack where manipulation is made to display a malicious website near the top of the results on a search website? 
a) Cross-site scripting b) DNS cache poisoning
c) SEO poisoning d) Social engineering 
( same with 2024 April 10.Q30 Security ( Attacking Poisoning) )

# 12 Q33.Security Information and Event Management ( SIEM )
Q33. Which of the following is a function of security information and event management (SIEM)?
a) The centralized control of a range of communication devices in a network, and the changing of network configuration and security settings 
EXPLANATION :: Network device control / configuration management (NAC-like function)

b) The execution of a file in an isolated virtual environment, and the monitoring of communication to a C&C server and other behavior 
EXPLANATION :: Sandbox analysis running files safely to observe malware behavior

c) The general analysis of logs that are collected from a range of devices, and the support of analysis and action by an administrator
EXPLANATION :: SIEM (log collection + analysis + alerting for security events) ✅

d) The inspection of header information in packets, the identification of application programs that receive communication, and the control of communication
EXPLANATION :: Firewall / deep packet inspection (controls traffic based on packet/application info)

# 13 Q44.System Relaibality
Q44. A device that operates 24 hours a day, 360 days a year has an MTBF value of 1,440
hours. Which of the following is the average number of failures for this device for 360 days?
Here, the result is rounded to the closest whole number, and the MTTR of the device is
ignored.
a) 3 b) 6 c) 9 d) 12 

# 14 Q47.System stretagy Service Oreinted Architecture
Q47. Which of the following is a description of the SOA?
a) A concept of constructing a system by considering the software functions as components
called services and combining them
b) A concept of improving sales efficiency and quality by using IT for sales activities to
increase sales and profits as well as to improve customer satisfaction
c) A concept of re-designing the business processes to innovatively improve the cost,
quality, service, and speed
d) Outsourcing the in-house operations that are not part of the core businesses to
concentrate the management resources on the core businesses

## EXPLANATION
a) SOA (Service-Oriented Architecture) → System built by combining reusable software “services”
b) CRM / Sales automation (improving sales using IT for customer satisfaction)
c) BPR (Business Process Reengineering) → Redesigning processes for major improvement in cost/quality/speed
d) Outsourcing → Giving non-core business work to external companies to focus on core work


# 15 Q48 System Stretagy  

Q48. Which of the following is the work that is performed when non-functional requirements
are defined?
a) Clarifying the flow of information (i.e., data) between the functions constituting business operations
b) Clarifying the interface for exchanging information with other systems
c) Creating the technical requirements for the development criteria and standards according to the programming language used in system development
d) Defining the scope to be implemented as system functions

## EXPLANATION
a) Data flow analysis (functional design – how data moves between business functions)
b) Non-functional requirements (system qualities like interfaces, performance, external system interaction) ✅
c) Development standards / technical rules (coding standards, language rules)
d) Functional requirements (what the system should do / scope of functions)


# 16 Q49 System Stretagy
Q49. Which of the following is an explanation of diversity management?
a) Both labor and management to reach an agreement on working conditions and work
together with the aim of increasing profits
b) For employees to harmonize between work and private life, approach their work with a
sense of purpose, and increase the vitality of the organization
c) For employees to take an autonomous approach to work with the aim of achieving the
objectives that they set for themselves and be evaluated according to the degree of
achievement
d) To increase the vitality of the organization by respecting the diversity among its
employees in terms of aspects such as gender, age, and nationality

## EXPLANATION
a) Labor-management cooperation (industrial relations / collective bargaining)
b) Work-life balance (harmony between work and private life)
c) Self-management / performance-based work (goal achievement & evaluation)
d) Diversity management (respecting differences like gender, age, nationality to improve organization vitality) ✅


