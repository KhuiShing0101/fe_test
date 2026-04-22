# 1
Q1. For an 8-bit binary integer, which of the following is the operation that extracts the most
significant 4-bits while making the other bits zero?
a) Bitwise AND operation with 11110000.
b) Bitwise NAND operation with 11110000.
c) Bitwise OR operation with 00001111.
d) Bitwise XOR operation with 00001111. 

**Correct Answer:** a) Bitwise AND operation with 11110000.

### Explanation
A bitwise **AND** operation keeps a bit as `1` only if both corresponding bits are `1`.

Using the mask `11110000`:
- The **most significant 4 bits (MSBs)** are preserved.
- The **least significant 4 bits (LSBs)** are set to `0`.

### Example
10101101 (original 8-bit number)
& 11110000 (mask)

10100000 (result)


### Why the Other Options Are Incorrect
- **b) NAND with 11110000** → Produces inverted AND result, not useful for masking.
- **c) OR with 00001111** → Forces last 4 bits to `1`, does not zero them.
- **d) XOR with 00001111** → Flips last 4 bits, does not zero them.

# 2 binary to decemal
Q2. Which of the following is the binary fraction that is the nearest equivalent to the decimal
fraction 23.375?
a) 10111.011 b) 10111.110 c) 11101.011 d) 11101.110 


### Explanation

Convert the decimal number 23.375 into binary:

1. Integer part (23 → binary)

23 ÷ 2 method:

23 → 10111
2. Fractional part (0.375 → binary)

Multiply by 2:

0.375 × 2 = 0.75   → 0
0.75  × 2 = 1.5    → 1
0.5   × 2 = 1.0    → 1

So:

0.375 → .011
Final Answer
23.375 = 10111.011
Why others are incorrect
b) 10111.110 → equals 23.75
c) 11101.011 → equals 29.375
d) 11101.110 → equals 29.75

So the nearest (and exact) binary equivalent is 10111.011.


# 3 
## Q10

The table below shows the access times for the cache memory and main memory in systems **A** and **B**. Which of the following is the approximate hit ratio of the cache memory, when the effective access time and the cache memory hit ratio are the same for systems **A** and **B**?

|                | System A | System B |
|----------------|----------|----------|
| Cache memory   | 14 ns    | 12 ns    |
| Main memory    | 80 ns    | 90 ns    |

**Options:**
- a) 0.17  
- b) 0.20  
- c) 0.83  
- d) 1.00  
**Answer:** c) 0.83  

**Short Explanation:**  
Use the Effective Access Time formula:  
\[
EAT = hT_c + (1 - h)(T_c + T_m)
\]

Since EAT is same for both systems, equate them and solve:  
\[
94 - 80h = 102 - 90h \Rightarrow h = 0.8
\]

Closest option ≈ **0.83**

# 4
Q15. When it takes 10 ns to copy a byte, which of the following is the approximate time (in
ms) to copy the data for a 1024 × 768-pixel graphics screen with 24-bit color? Here, any
overhead time for copying can be ignored.
a) 22 b) 23 c) 24 d) 25 


# 5 
Q23. Which of the following is the most appropriate information for a router to determine the destination of an incoming packet?
a) Destination IP address b) Destination MAC address
c) Source IP address d) Source MAC address 

**Answer:** a) Destination IP address  

**Short Explanation:**  
A router operates at the **network layer (Layer 3)** and uses the **destination IP address** to decide where to forward a packet.  
MAC addresses are used only within a local network (by switches), not for routing between networks.

# 6 OSI model Knowledge
Q24. In the OSI model, which of the following is the layer that is responsible for routing
datagrams between hosts utilizing IP addresses across one or more networks?
a) Data link b) Network c) Physical d) Transport

**Answer:** b) Network  

**Short Explanation:**  
The **Network layer (Layer 3)** of the OSI model is responsible for **routing datagrams** using **IP addresses** across multiple networks.

# 7 Address Resolution
Q25. Which of the following is an appropriate explanation regarding Address Resolution
Protocol (ARP)?
a) It converts MAC addresses into IP addresses.
b) It resolves domain names into its IP addresses.
c) It resolves IP addresses into the corresponding MAC addresses.
d) It translates IPv4 addresses into IPv6 addresses.

**Answer:** c) It resolves IP addresses into the corresponding MAC addresses.  

**Short Explanation:**  
ARP maps a device’s **IP address to its MAC address**, enabling communication within a local network.

# 8 Small Network
## Q26

An administrator of a small network is testing the new network. Which of the following is the correct combination of the network management tools to be inserted in the blanks below?

The administrator first tests reachability of a remote host using **A**, and determines the path that packets take to the destination with **B**.

| Option | A        | B           |
|--------|----------|-------------|
| a)     | netstat  | ping        |
| b)     | netstat  | traceroute  |
| c)     | ping     | traceroute  |
| d)     | traceroute | ping      |

### explination

**Short Explanation:**
- **a)** ❌ netstat shows connections, ping tests reachability → wrong order  
- **b)** ❌ netstat not used for reachability testing  
- **c)** ✔️ ping checks reachability, traceroute finds path → correct  
- **d)** ❌ traceroute finds path, ping checks reachability → wrong order  

# 9 DNS posining
## Q27. Which of the following is the attack that is classified as DNS cache poisoning?

a) False domain information is injected into the DNS server that is referenced by a PC, and
it leads the user to a fake server.
b) In order to interrupt the target service, the attacker uses the DNS server as a
steppingstone to send a large number of recursive queries.
c) In order to obtain internal information, the zone information stored in the DNS server is
compiled and transferred.
d) The version information of the DNS server software is obtained to identify a security
hole. 

**Answer:** a) False domain information is injected into the DNS server that is referenced by a PC, and it leads the user to a fake server.

## explanation
**Short Explanation:**
- **a)** ✔️ DNS cache poisoning → fake IP is stored, redirects users to malicious sites  
- **b)** ❌ DNS amplification (DDoS attack)  
- **c)** ❌ DNS zone transfer (information gathering)  
- **d)** ❌ DNS fingerprinting (version detection for vulnerabilities)  


# 9 
Q41. Which of the following is an appropriate explanation of earned value in project
management?
a) A measure of work completed in terms of budget authorized for that work.
b) A time-phased budget that estimates the total cost of a project
c) An authorized budget for the planned work
d) Realized cost incurred for the work performed on an activity during a specific time
period 

## explanation

**Explanation:**
- **a)** ✔️ **Earned Value (EV)** → shows how much work is completed, expressed in terms of approved budget  
- **b)** ❌ **Planned Value (PV)** → planned/expected budget over time  
- **c)** ❌ **Budget at Completion (BAC)** → total planned project budget  
- **d)** ❌ **Actual Cost (AC)** → actual money spent  

**Answer:** a) A measure of work completed in terms of budget authorized for that work.
👉 So, **Earned Value = value of work actually completed (in budget terms)**.



# 10 COCOMO model in software estimation
Q42. Which of the following is the method of estimation in the COCOMO model in software
estimation?
a) The effort and duration of the project are estimated based on the size of the software.
b) The effort of the project is estimated based on the duration of the project.
c) The size of the software and duration of the project are estimated based on the effort of
the project.
d) The size of the software and effort of the project are estimated based on the duration of
the project. 

**Short Explanation:**
- **a)** ✔️ COCOMO → estimates effort & time using software size (e.g., KLOC)  
- **b)** ❌ Duration is derived from effort, not the other way  
- **c)** ❌ Size is an input, not estimated from effort  
- **d)** ❌ Duration is not the primary input in COCOMO  

**Answer:** a) The effort and duration of the project are estimated based on the size of the software.

# 11
Q43. An IT service is provided under the conditions below. What is the maximum downtime in hours that satisfies the SLA during a service period of one (1) month? Here, the number of business days in one (1) month is 30, and no maintenance or other scheduled downtime of the service is performed during the service period. [Conditions of the SLA] - The service period is from 8:00 AM to 10:00 PM on business days. - The availability should be 99.5% or more. 

a) 0.3 b) 2.1 c) 3.0 d) 3.6

### Explanition

**Short Explanation:**
- Service hours per day = 8 AM → 10 PM = **14 hours**  
- Monthly service hours = \( 14 \times 30 = 420 \) hours  
- Allowed downtime = \( 0.5\% \) of 420  
\[
= 0.005 \times 420 = 2.1 \text{ hours}
\]

👉 Maximum downtime = **2.1 hours**

# 12
Q44. Which of the following should be accomplished in service management concerning
Maximum Tolerable Downtime (MTD), Recovery Point Objective (RPO), and Recovery
Time Objective (RTO)?
a) MTD < RPO b) MTD < RTO c) RPO < MTD d) RTO < MTD 

### Explanition
**Short Explanation:**
- **MTD (Maximum Tolerable Downtime)** → max time system can be unavailable  
- **RTO (Recovery Time Objective)** → time to restore service  

👉 Recovery must happen **before** maximum tolerable downtime is exceeded  
So: **RTO < MTD**

- **a)** ❌ no direct relation  
- **b)** ❌ wrong (MTD is larger)  
- **c)** ❌ RPO relates to data loss, not downtime limit  
- **d)** ✔️ correct  


# 13 checkpoint for auditing 
Q45.Which of the following is a checkpoint for auditing the control of risks related to
information leakage and unauthorized use of documents concerning a system?
a) Creating the necessary documents even in prototype development
b) Standardizing documents
c) Taking measures to ensure the confidentiality of documents
d) Updating documents without delay as changes are made in the system

### Explanition
**Short Explanation:**
- **a)** ❌ focuses on documentation creation, not security risks  
- **b)** ❌ standardization ≠ protection from leakage  
- **c)** ✔️ directly addresses **information leakage & unauthorized use**  
- **d)** ❌ about maintenance/updates, not confidentiality  

👉 For auditing risk control, **confidentiality is the key factor**
**Answer:** c) Taking measures to ensure the confidentiality of documents 

# 14 Facilitator
Q57. Which of the following is the appropriate role of a facilitator in a meeting?
a) To act as the chairperson and control the discussions in order to work out a conclusion
that matches the intentions of the management
b) To encourage the meeting participants to express their opinions and organize the flow
of discussions from a neutral and impartial position
c) To offer specialized support for meeting administration, such as adjusting the schedule,
preparing materials, or taking minutes.
d) To provide advice only on discussions related to specific areas in which the facilitator
specializes, such as technical or legal fields 

### Explanition

**Short Explanation:**
- **a)** ❌ biased toward management, not neutral  
- **b)** ✔️ facilitator = **neutral guide**, encourages participation  
- **c)** ❌ administrative/support role (secretary)  
- **d)** ❌ expert/advisor role, not facilitator  

**Answer:** b) To encourage the meeting participants to express their opinions and organize the flow of discussions from a neutral and impartial position  
👉 Key point: facilitator ensures **fair, balanced, and productive discussion**

# 15 fishbone diagram ( cause and eff diagram )
Q58. The figure below shows part of a cause and effect diagram (also known as a fishbone
diagram). Which of the following is the relationship between A and B
    ────────────────▶ A
           ▲
           │
           B
a) B is an attribute of A. b) B is the cause of A.
c) B is the means of A. d) B is the purpose of A. 

### Explanition
**Short Explanation:**
- **a)** ❌ Attribute = characteristic, not causal relationship  
- **b)** ✔️ Fishbone diagram shows **cause → effect**, so B causes A  
- **c)** ❌ Means = method to achieve something, not shown here  
- **d)** ❌ Purpose = goal, not a cause-effect link  

👉 In a cause-effect (fishbone) diagram: **branches = causes**, **head = effect**

**Answer:** b) B is the cause of A  

# 16 Data mining and process mining ( cause and eff diagram )

Q59. Both Data mining and Process mining are methods for improving business operations.
While Data mining aims to discover knowledge by analyzing large amounts of data by using
statistical and AI analysis methods, which of the following is an appropriate explanation of
Process mining?
a) It is a management strategy focused on changing workflows and business processes
within an organization by emphasizing new ideas and new ways of doing business.
b) It is a method aimed at analyzing data sets, finding unsuspected relationships, and
summarizing the data in novel ways.
c) It is a methodology for improving performance by systematically removing unnecessary
data.
d) It is a technique for analyzing and improving business processes by using knowledge
that is extracted from event logs. 

### **Short Explanation:**
- **a)** ❌ Business Process Reengineering (BPR), not process mining  
- **b)** ❌ Data mining definition  
- **c)** ❌ Data cleaning/reduction, not process mining  
- **d)** ✔️ Process mining → uses **event logs** to analyze & improve processes  

**Answer:** d) It is a technique for analyzing and improving business processes by using knowledge that is extracted from event logs.  

👉 Key idea: **Process mining = event log–based process analysis**


# 17 Salvage value
Q60. Company A purchased a machine for an original cost of $126,000. The salvage value
after 6 years is $6,000. What is the annual depreciation expense (in dollars) by using the
straight-line method?
a) 12,000 b) 20,000 c) 21,000 d) 36,000

###

**Short Explanation:**
- **a) 12,000** ❌ incorrect calculation  
- **b) 20,000** ✔️ \((126,000 - 6,000) / 6 = 20,000\)  
- **c) 21,000** ❌ miscalculation  
- **d) 36,000** ❌ ignores proper straight-line formula  

👉 Formula: \((\text{Cost} - \text{Salvage}) / \text{Life}\)
