# 1 OR GATE 
### Q1. P, Q, and R are propositions. It is known that the truth value of proposition P is true, and
the values of both the propositions “(not P) or Q” and “(not Q) or R” are true. Which of the
following is a combination of the truth values of Q and R? Here, X or Y represents the
logical sum of X and Y, and not X represents the negation of X.
Q R
a) False False
b) False True
c) True False
d) True True

Let’s solve step by step 👇

🔹 Given:
P = True
🔹 Statement 1:

(not P) or Q = True

not P = False (since P is True)
👉 So: False OR Q = True
👉 This is only possible if Q = True
🔹 Statement 2:

(not Q) or R = True

Q = True → not Q = False
👉 So: False OR R = True
👉 This is only possible if R = True
A / B / C / D format:
A ❌ (False, False) → Q wrong
B ❌ (False, True) → Q wrong
C ❌ (True, False) → R wrong
D ✔ (True, True) → Correct
🔹 Final Answer: D

# 2 CPU Avg Access Time
### Q9. When the CPU needs data, it first accesses the cache memory. When the data is not
available in the cache memory, the CPU accesses the main memory. If the miss ratio is 0.2
and the access times for cache memory and main memory are as shown below, what is the
approximate average memory access time in ns for the CPU? Here, there are only cache
memory and main memory for the CPU, the access time for main memory includes the time
to confirm whether the data is available in cache memory, and the overhead time for the
cache management can be ignored.
Access destination Access time (ns)
Cache Memory 75
Main Memory 1500
a) 315 b) 360 c) 1,215 d) 1,260

🔹 1. Hit Ratio & Miss Ratio
Hit Ratio → Data found in cache (fast)
Miss Ratio → Data NOT found in cache (slow)

👉 Relation:

Hit Ratio + Miss Ratio = 1

🔹 Super short memory:
Hit × cache time → fast part
Miss × memory time → slow part
Add them → average time

# 3
### Q16. A graphical symbol for the 2-to-1 MUX (multiplexer) and its truth table are shown in
the figure below. The MUX has two data inputs (I0, I1), one select-line (S) and one output
(Z). If the select line is S=0, then the output Z is switched to input I0, whereas if a select line
is S=1, then the output Z is switched to input I1.
Which of the following is a logic gate that is equivalent to the circuit implemented with the
2-to-1 MUX below? 
(Q16.png)

2-to-1 MUX behaves like XOR gate

Given:

When X₁ = 0, output Y = X₂
When X₁ = 1, output Y = X₂̅ (NOT X₂)
Compare with XOR behavior

A XOR gate works like this:

If X₁ = 0 → output = X₂
If X₁ = 1 → output = NOT X₂
Conclusion

Since the MUX output matches exactly with XOR behavior:

Y = X₁ ⊕ X₂

Final Answer:

d) XOR gate

same = 0 , not same = 1

| Gate | “Opposite” / Related form |
| ---- | ------------------------- |
| OR   | NOR (inverted OR)         |
| AND  | NAND (inverted AND)       |
| XOR  | XNOR (true complement)    |


# 4 OSI model layers
OSI Model Layers (1 to 7)
Physical Layer → cables, signals, repeaters
Data Link Layer → MAC addresses, switches, bridges
Network Layer → IP addresses, routers
Transport Layer → TCP/UDP, end-to-end delivery
Session Layer → manages sessions/connections
Presentation Layer → data format, encryption, compression
Application Layer → user services (HTTP, FTP, email, etc.)

### Q23. Which of the following is an appropriate description of a device that connects LANs?
a) A bridge relays frames based on IP addresses.
b) A gateway converts the protocols of only the first through third levels in the OSI basic
reference model.
c) A repeater extends the transmission distance by amplifying signals between segments of
the same type.
d) A router relays frames based on MAC addresses. 


# broadcast address
Q24. What is the broadcast address of the network 192.168.128.0/22?
a) 192.168.128.127 b) 192.168.128.255
c) 192.168.131.255 d) 192.168.255.255 

📌 Given:

Network: 192.168.128.0/22

🧠 Step 1: Understand /22 subnet
/22 means subnet mask = 255.255.252.0
Block size in 3rd octet = 256 − 252 = 4

So networks increase like:

192.168.128.0
192.168.132.0
192.168.136.0 …
📌 Step 2: Find the range of this subnet

Start network:

192.168.128.0

Next network:

192.168.132.0

So this subnet covers:

From 192.168.128.0
To 192.168.131.255
📡 Step 3: Broadcast address

Broadcast = last address of the range

👉 192.168.131.255

✔️ Final Answer:

c) 192.168.131.255

