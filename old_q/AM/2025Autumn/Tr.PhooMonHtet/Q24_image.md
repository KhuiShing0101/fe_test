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


# 4 Avrage Access Time CPU
Q9.When an HDD has the specifications shown in the table below, what is the average access
time for the HDD to transfer 16 kB of data in milliseconds (ms)? The average access time is
calculated as the sum of the average seek time, controller overhead, rotational latency, and
transfer time. Other overheads can be ignored. Here, 1 MB = 1,024 kB.

Average seek time5 ms
Rotation Speed6,000 RPM
Transfer rate1 MB/s
Controller overhead0.1 ms

a) 20.1
b) 25.725
c)30.725
d) 74.1

### Let’s compute it step by step (short and clear):

1. Given:

Seek time = 5 ms
Controller overhead = 0.1 ms
Rotation speed = 6000 RPM
Transfer rate = 1 MB/s
Data = 16 kB

2. Rotational latency

6000 RPM = 6000 / 60 = 100 rotations/sec
Time per rotation = 1 / 100 = 10 ms
Average latency = 10 / 2 = 5 ms

3. Transfer time

1 MB = 1024 kB
Time to transfer 16 kB = 16 / 1024 = 0.015625 s = 15.625 ms

4. Total access time
= Seek + Latency + Transfer + Overhead
= 5 + 5 + 15.625 + 0.1
= 25.725 ms

✅ Correct answer: b) 25.725 ms

# 5 3D printers
Q10.Which of the following is an appropriate description of a 3D printer’s function?
a) It detects the shape of three-dimensional objects and produces output of 3D data.
b) It functions by pushing the pins of a high-temperature printing head onto heat-sensitive
paper.
c) It makes three-dimensional objects using methods such as fused filament fabrication.
d) It projects computer graphics onto uneven three-dimensional objects such as buildings
and furniture.

### Explaination
a) Describes a 3D scanner, not a printer (it captures shapes, doesn’t create objects).
b) Describes a thermal printer, which uses heat on special paper.
c) ✅ Correct — A 3D printer creates physical 3D objects, commonly using methods like fused filament fabrication (FFF).
d) Describes projection mapping, not printing.

# 6 Logical Circuit!
Q16.Which of the following is equivalent to the logical circuit shown below?
[Q16 logical circuit ](quition16.png) 
a) A · B  
b) Ā · B  
c) A · B̄  
d) Ā · B̄
### Q16 Explanation

**Step 1: Top branch**
- A passes through NOT → Ā  
- Then AND with B → Ā · B  

**Step 2: Bottom branch**
- A and B go into NOR → (A + B)̄  

**Step 3: Final output**
Y = ((Ā · B) + (A + B)̄)̄  

**Step 4: Simplify**
(A + B)̄ = Ā · B̄  

Y = ((Ā · B) + (Ā · B̄))̄  
Y = (Ā (B + B̄))̄  
Y = (Ā · 1)̄  
Y = (Ā)̄ = A  

**Final Answer:**  
Y = A

# 7 prioritize traffic  
Q23. Which of the following is a mechanism used to prioritize traffic based on its importance
and minimize network latency for network applications?
a) AAA
b) PoE
c) QoS
d) RTP

### Q23 Answer

**Correct Option:** c) QoS

### Short Explanation

- **QoS (Quality of Service)** prioritizes important network traffic and reduces delay (latency), ensuring better performance for applications like video calls and gaming.

### Why others are incorrect

- **AAA** → Authentication, Authorization, Accounting (security-related)  
- **PoE** → Power over Ethernet (supplies power, not traffic control)  
- **RTP** → Real-time Transport Protocol (used for media streaming, not prioritization)

# 8  ARP behavior Broadcast
Q24. PC5 has been newly added to the network. It wants to send data to PC4 using SSH
protocol. It must resolve the MAC address of PC4 from its IP address before sending the data.
Which of the following is the destination MAC address that PC5 will use in ARP request?
![Q 24](image.png)

a) 00:00:00:00:00:00
c) 78:E1:00:3C:A1:9F
b) 78:E1:00:3C:A1:8B
d) FF:FF:FF:FF:FF:FF

### Explanation (ARP behavior) 

When PC5 (192.168.1.11) wants to send data to PC4 (192.168.1.10), it must first find PC4’s MAC address using ARP.
Since PC5 does not yet know the MAC of PC4, it sends an ARP request to the local network using a broadcast MAC address so that all devices receive it.
ARP Request Destination MAC = Broadcast address

Broadcast MAC is:

FF:FF:FF:FF:FF:FF

Only PC4 will respond with its actual MAC address, while all other devices ignore the request.

Final Answer (copy-ready)
d) FF:FF:FF:FF:FF:FF

# 9 OSI Layer
Q25. Between LAN systems that are different from the transport layer upward in the OSI basic reference model, which of the following is a device that performs protocol conversion? 
a) Bridge b) Gateway c) Repeater d) Router

### Explanation
A gateway is the device that performs protocol conversion between different network systems, especially when the systems differ from the transport layer upward in the OSI model. It can translate between different communication protocols and architectures.
Quick comparison:
Repeater → Works at Physical layer (Layer 1), regenerates signals only
Bridge → Works at Data Link layer (Layer 2), connects LAN segments
Router → Works at Network layer (Layer 3), routes packets between networks
Gateway → Works across higher layers (Transport and above) and performs protocol conversion
So the best answer is Gateway.

# 10 
Q26. Which of the following is an Internet standard that extends the format of email header
fields to handle not only text messages but also audio and image files?
a) HTML
b) MHS
c) MIME
d) SMTP

MIME (Multipurpose Internet Mail Extensions) is the Internet standard that extends email format so it can carry not only plain text but also audio, images, video, and other file types. It works alongside email protocols like SMTP to allow attachments and rich content in emails.

Quick clarity on the options:

HTML → Markup language for web pages, not an email standard
MHS → Message Handling System (older X.400 email system)
MIME → ✅ Extends email to support multimedia content
SMTP → Simple Mail Transfer Protocol, used only for sending email, not handling attachments

So, the correct choice is MIME.

# 11 Critical Path
Q48 Eight (8) activities and milestones of a project are shown in the arrow diagram below.
Which of the following is the critical path of this project?

![critical_path](Q41.png)

a) A, C, E, H
b) A, C, F, G
c) B, E, H
d) B, F, G

# 12 
Q42. Based on the requirements gathered, the cost of a software project under normal
conditions is estimated at $70,000. In case of smooth project implementation, some activities
are not required and the estimated cost is reduced to $50,000; however, in the worst-case
scenario, additional tasks are required and the cost increases to $120,000. What is the
expected cost of the project (in dollars) that is calculated by using the three-point estimate in
the beta distribution, also known as PERT?
a) 70,000
b) 75,000
c) 80,000
d) 85,000