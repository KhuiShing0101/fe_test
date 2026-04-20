# 1.Q5 double link list
## Q5 The table below shows the data in a list structure that has bidirectional pointers. In this table, a new Employee **G** is to be inserted between Employee **A** and Employee **K**. 

Which of the following contains only the pointers (among **a** through **f**) whose values change after the insertion?

---

### Table (Before Insertion)

| Address | EmployeeName | NextPointer | PreviousPointer |
|--------:|--------------|-------------|-----------------|
| 100     | Employee A   | 300         | 0               |
| 200     | Employee T   | 0           | 300             |
| 300     | Employee K   | 200         | 100             |

---

### Table (After Insertion)

| Address | EmployeeName | NextPointer | PreviousPointer |
|--------:|--------------|-------------|-----------------|
| 100     | Employee A   | a           | b               |
| 200     | Employee T   | c           | d               |
| 300     | Employee K   | e           | f               |
| 400     | Employee G   | x           | y               |

---

### Options

a) a, b, e, f  
b) a, e, f  
c) a, f  
d) b, e  

## Linked List (Short Note)

A **Linked List** is a linear data structure where elements (called *nodes*) are stored in non-contiguous memory locations. Each node contains:
- **Data**
- **Pointer(s)** to the next (and sometimes previous) node

### Types of Linked Lists
- **Singly Linked List**: Each node points to the next node.
- **Doubly Linked List**: Each node has pointers to both next and previous nodes.
- **Circular Linked List**: Last node points back to the first node.

### Key Features
- Dynamic size (can grow/shrink easily)
- Efficient insertion and deletion (no shifting required)
- Sequential access (no direct indexing like arrays)

### Basic Operations
- **Insertion** (beginning, middle, end)
- **Deletion**
- **Traversal** (visiting each node)
- **Searching**

### Advantages
- Flexible memory usage
- Efficient insert/delete operations

### Disadvantages
- No random access (must traverse)
- Extra memory needed for pointers
- More complex than arrays

### Example (Singly Linked List)
A → B → C → D → NULL


# 2 Q6 GCD greatest common divisor
Example:

x = 12, y = 18
Common divisors: 1, 2, 3, 6
GCD = 6

## Q6 The flowchart shown below expresses an algorithm that determines the greatest common divisor between two integers **a** and **b**.  
How many times is **A** passed?

---

**Flowchart (Euclidean Algorithm):**

Start  
↓  
a ← 56  
b ← 48  
↓  

Repeat:
- r ← a mod b  
- a ← b  
- b ← r  
- If r ≠ 0 → pass through **A** and repeat  
- If r = 0 → print a and end  

---

### Step-by-step execution

1. **First pass**
   - r = 56 mod 48 = 8  
   - a = 48, b = 8  
   - r ≠ 0 → pass A (**1 time**)

2. **Second pass**
   - r = 48 mod 8 = 0  
   - a = 8, b = 0  
   - r = 0 → stop (no pass through A)

---

### Final Answer

**A is passed 1 time**

---

**Correct option: a) 1**

# 3 Q10  
## Q10. Which of the following is an appropriate description of a 3D printer’s function?
a) It detects the shape of three-dimensional objects and produces output of 3D data.
b) It functions by pushing the pins of a high-temperature printing head onto heat-sensitive
paper.
c) It makes three-dimensional objects using methods such as fused filament fabrication.
d) It projects computer graphics onto uneven three-dimensional objects such as buildings
and furniture. 
a) ❌
Describes a 3D scanner, not a printer (it captures shape/data, doesn’t create objects).

b) ❌
Describes thermal or dot-matrix printing, which prints on paper — not 3D objects.

c) ✅
Correct — methods like fused filament fabrication (FFF) are standard in 3D printing.

d) ❌
Describes projection mapping, used for visuals on surfaces, not printing objects.

# 4 Q11
## Q11. Which of the following is the most appropriate explanation of edge computing?
a) Increasing the operability and expressiveness of web application software by performing
screen creation and data processing on the client side
b) Increasing the real-time nature of processing by performing primary processing of data
on a server or other such computer in a location close to the origin of data, such as a
sensor that is attached to a user or a device
c) Increasing throughput with parallel processing by virtualizing and integrating several
servers and PCs and creating a single high-performance computer
d) Starting up the required server only when data comes in, and freeing up resources by
stopping the server as soon as the processing is finished 

a) ❌
Describes client-side processing in web apps (like JavaScript in a browser), not edge computing.

b) ✅
Correct — edge computing reduces latency by handling data locally/nearby.

c) ❌
Describes cluster computing / parallel processing, combining machines for performance.

d) ❌
Describes serverless computing (on-demand servers), not edge computing.

# 5 Q12
## Q12

One (1) server, three (3) clients, and two (2) printers are connected via a LAN as shown below.  
This system prints data located on the server in response to instructions from the clients.

When the availability of each device is as shown in the table below, which of the following expressions represents the availability of the system?

> The system is considered **available** if:
> - One (1) of the three (3) clients is running, and  
> - One (1) of the two (2) printers is running.

---

### Availability Table

| Device  | Availability |
|--------|-------------|
| Server | a           |
| Client | b           |
| Printer| c           |
| LAN    | 1           |

              [Server]
                 |
-------------------------------------
 |      |      |      |       |
C1     C2     C3     P1      P2

---

### Options

a) \( ab^3 c^2 \)  
b) \( a (1 - b^3)(1 - c^2) \)  
c) \( a (1 - b)^3 (1 - c)^2 \)  
d) \( a \big(1 - (1 - b)^3\big)\big(1 - (1 - c)^2\big) \)

✔️ Correct answer: d) a(1 - (1 - b)^3)(1 - (1 - c)^2)

---

### Short explanation:

- Server works → probability = a  
- At least 1 of 3 clients works → 1 - (1 - b)^3  
- At least 1 of 2 printers works → 1 - (1 - c)^2  

---

### Final expression:

a × (1 - (1 - b)^3) × (1 - (1 - c)^2)

✔️ Answer: d

# 6 Q27
## Q27. An attacker left a USB stick labeled “Next ITPEC exam questions and answers” that
contains malware in front of an office, expecting someone to plug it into a PC. Once plugged
in, the attacker gains control of the PC. Which of the following types of attack is this?
a) Baiting b) Identity theft
c) Phishing d) Pretexting 


a) Baiting ✅ (Correct answer)

This is an attack where the attacker uses something tempting or attractive (a “bait”) to trick the victim into taking an action.

Example: Leaving a USB stick labeled “Exam answers” or “Free movies”
Victim plugs it in → malware installs → attacker gains access

👉 Key idea: temptation + infected device or download

✔️ This question is exactly baiting.

b) Identity theft

This is when someone steals personal information (like name, passwords, ID numbers) and uses it as if they are that person.

Example: Using someone’s credit card or login credentials
Focus: stealing identity data, not tricking via devices

❌ Not related to USB trap scenario

c) Phishing

This is when attackers use fake emails, messages, or websites to trick people into giving sensitive information.

Example: Fake bank email asking for password
Usually involves links or login pages

❌ No email or fake website here → not phishing

d) Pretexting

This is when the attacker pretends to be someone else to gain trust and extract information.

Example: Calling as “IT support” asking for your password
Focus: fake identity + conversation

❌ No impersonation in this question

✔️ Final Answer:

a) Baiting


# 7 Q28 
## Q28. When X receives a message with a digital signature that uses public key cryptography
from Y, which of the following is the key that X uses to verify that the message truly came
from Y?
a) X’s private key b) X’s public key
c) Y’s private key d) Y’s public key 
Short note:

In digital signatures:

Y signs the message using Y’s private key
X verifies the signature using Y’s public key

👉 This proves the message really came from Y and wasn’t changed.

✔️ Final Answer: d) Y’s public key

# 8 Q29 DNS Cache Posining
## Q29.The IP address of server X that is owned by an attacker, is recorded on Company B’s
DNS cache server as the IP address corresponding to the FQDN of Company A’s web server.
As a result, which of the following are the users that unintentionally connect to server X?
Here, the employees of Company A and Company B use their own company’s DNS cache
server for name resolution.
a) Company A employees who try to connect to Company A’s web server
b) Company A employees who try to connect to Company B’s web server
c) Company B employees who try to connect to Company A’s web server
d) Company B employees who try to connect to Company B’s web server 

🔑 Short note:
This is a DNS cache poisoning attack.

Company B’s DNS cache is poisoned
It stores fake IP (attacker’s server X) for Company A’s web server name
So when Company B employees try to access Company A’s website, they are redirected to server X
✔️ Final Answer: c)

# 8 Q30 fraud triangle
## Q30. When a fraud occurs, all three (3) elements of the “fraud triangle” are believed to exist.
Which of the following is the appropriate explanation of an element of the “fraud triangle”?

a) “Information and communication” refers to the identification, understanding, and
processing of the required information, and its proper communication both within and
outside the organization, and among the concerned persons.
b) “Opportunity” refers to the existence of an environment, such as technologies like the
information system, physical environment, organizational rules, etc., that makes fraud
possible or easy to commit.
c) “Pressure,” also known as incentive or motivation, refers to the selfish reasoning to
justify committing fraud, such as interpreting things in a way that overcomes guilt or
shifts blame.
d) “Rationalization” refers to the feeling of being forced caused by unrealistic performance
targets.

🔑 Short explanation (Fraud Triangle):

The fraud triangle has 3 elements:

Pressure (Incentive)
Opportunity
Rationalization
✔️ Option check:
a) ❌ Wrong
This describes information systems / communication process
Not part of fraud triangle
b) ✔️ Correct
Opportunity = conditions that allow fraud
Example:
weak security systems
poor controls
lack of supervision
Makes fraud possible or easy to commit
c) ❌ Wrong
This actually describes Rationalization, not Pressure
Rationalization = “justifying wrongdoing”
d) ❌ Wrong
This describes Pressure, not Rationalization
Pressure = financial stress, targets, debt, etc.
✔️ Final Answer: b)

# 9 Q31 IDS Intrusion Detection System
## Q31. Which of the following is a function of an IDS?
a) It checks whether software products that are installed on a PC are the latest version.
b) It collects the status of information security measures, such as the status of operations
management for an information system, and also obtains company information, then
performs a self-diagnosis on the status of activities for information security in an
organization.
c) It monitors a server or a network and notifies the administrator when it has detected an
intrusion or infringement.
d) It sends test data to a product that it examines and detects any vulnerability from the
response or behavior of the product. 

✔️ Correct answer: c)
🔑 Short note:

An IDS (Intrusion Detection System) is used to:

👉 Monitor networks or systems and alert when suspicious or malicious activity is detected

✔️ Option check:
a) ❌ Wrong
This is software update checking
Not IDS function
b) ❌ Wrong
This describes security auditing / management assessment
Not real-time intrusion detection
c) ✔️ Correct
IDS monitors network or server activity
Sends alerts when intrusion is detected
d) ❌ Wrong
This describes a vulnerability scanner
It actively tests systems for weaknesses, not just detects intrusions
✔️ Final Answer: c)

# 10 Q32 Attacker Port Scanning
## Q32. Which of the following is an appropriate description concerning the timing and purpose
of port scanning when an attacker intrudes into a system?
a) It is conducted at the post-processing stage in order to look for any evidence of attack
that may remain in the system log.
b) It is conducted at the preliminary investigation stage in order to look for any service that
can be attacked.
c) It is conducted at the privilege escalation stage in order to look for any account whose
privileges can be obtained.
d) It is conducted at the unauthorized action stage in order to look for any user information
that may be beneficial to the attacker. 

🔑 Short note:

Port scanning is usually done at the reconnaissance / initial stage of an attack.

👉 Purpose:
To find open ports and running services that can be exploited.

✔️ Option check:
a) ❌ Wrong
This is post-attack analysis (forensics/log review)
Not port scanning
b) ✔️ Correct
Port scanning is done in the preliminary investigation stage
Used to identify vulnerable services
c) ❌ Wrong
This is privilege escalation stage
Not related to scanning ports
d) ❌ Wrong
This describes data theft stage
Not port scanning
✔️ Final Answer: b)

# 11 Web Application Firewall ( WAF )
## Q33. In a system with the configuration and communication services shown in the figure below,
which of the following is the most appropriate location for the installation of a WAF as a
countermeasure for a vulnerability in a web application? Here, the WAF has no function to
encrypt or decrypt communications. 

### System Diagram

      [PC]   [PC]   [PC]
        \     |     /
        [  Internet  ]
              |
          (HTTPS / A)
              |
        [  Firewall  ]
              |
          (HTTPS / B)
              |
      [ SSL Accelerator ]
              |
           (HTTP / C)
              |
        [ Web Server ]
              |
      (Service Access / D)
              |
      [ Database Server ]
    a) A b) B c) C d) D

A / B / C / D format:

A: Before firewall, encrypted (HTTPS) → WAF cannot inspect ❌
B: After firewall but still encrypted (HTTPS) → WAF cannot inspect ❌
C: After SSL Accelerator, decrypted (HTTP) → WAF can inspect ✔ (Correct)
D: After web server, too late for protection ❌

# 12 feasibility
## Q46. Which of the following is an appropriate feasibility evaluation when checking whether
the lifetime benefits of the proposed information system are greater than its lifetime costs?
a) Economic feasibility b) Operational feasibility
c) Scheduling feasibility d) Technical feasibility 

Answer: a) Economic feasibility

A / B / C / D format:

A: Economic feasibility ✔ → Checks whether lifetime benefits are greater than lifetime costs (cost–benefit analysis).
B: Operational feasibility ❌ → Checks whether the system will work in the organization and be accepted by users.
C: Scheduling feasibility ❌ → Checks whether the project can be completed within the required time.
D: Technical feasibility ❌ → Checks whether the required technology and skills are available.

Final Answer: A

# 13 System reliablility
## Q47. Which of the following is a measure for the risk of a decline in the system maintenance
and operation quality during the outsourcing of an IT service?
a) Clearly stating the detailed fee structure by service in the contract or other documents,
in order to validate the service costs
b) Requesting a proposal for the human resource development plan of the company after
outsourcing during the stage of subcontractor selection, and clearly stating it in the
contract or other documents
c) Securing human resources with capabilities to evaluate the appropriateness of service
costs for system maintenance and operation within the company
d) Using indexes that demonstrate the service quality in order to promote improvement
activities after agreeing on the desired level of quality with the subcontractor 

Answer: d) Using indexes that demonstrate the service quality in order to promote improvement activities after agreeing on the desired level of quality with the subcontractor

A / B / C / D format:

A ❌ → Focuses on cost transparency, not service quality control.
B ❌ → HR development planning is indirect and not a direct measure of service quality risk.
C ❌ → Internal staffing for cost evaluation does not directly ensure outsourced service quality.
D ✔ → Uses service quality metrics (KPIs/SLAs) and continuous monitoring/improvement, which directly prevents decline in maintenance and operational quality during outsourcing.

# 14 Flow Diagram
## Q48. In a business scenario where marketing managers analyze customer interests and sales
patterns, design promotional campaigns, and then send targeted emails to customers, which
of the following is a modeling technique used to represent how information flows between
internal processes, data stores, and external entities?
a) Class Diagram b) Data Flow Diagram (DFD)
c) Entity-Relationship Diagram (ERD) d) Use Case Diagram

Answer: b) Data Flow Diagram (DFD)

A / B / C / D format:

A ❌ Class Diagram → Shows structure of objects/classes in object-oriented design, not data flow.
B ✔ Data Flow Diagram (DFD) → Represents how data moves between processes, data stores, and external entities (fits the scenario).
C ❌ Entity-Relationship Diagram (ERD) → Models database structure (entities and relationships), not process flow.
D ❌ Use Case Diagram → Shows system functionality from a user perspective, not detailed data movement.

Final Answer: B

# 15  benchmarking 
## Q49. Which of the following is an explanation of benchmarking that is used for corporate
management?
a) It refers to a qualitative and quantitative understanding of a company’s own products,
services, and operations through comparison with those of competitors or advanced
companies.
b) It refers to drastically reforming the quality and structure of a company by redesigning
its business processes from a customer viewpoint and by taking full advantage of
information technology.
c) It refers to the ability to plan and manage the allocation of company-wide management
resources in an effective and integrated manner in order to improve management
efficiency.
d) It refers to the concentration of management resources on the unique skills and
technologies of a company that can generate profit and that are superior to those of other
companies.

Answer: a) It refers to a qualitative and quantitative understanding of a company’s own products, services, and operations through comparison with those of competitors or advanced companies.

A / B / C / D format:

A ✔ Benchmarking → Comparing your company’s performance with competitors or best-in-class organizations to identify gaps and improve.
B ❌ Business Process Reengineering (BPR) → Radical redesign of business processes using IT.
C ❌ ERP / resource management concept → Integrated planning and management of enterprise resources.
D ❌ Core competence strategy → Focusing on unique strengths to gain competitive advantage.

Final Answer: A

# 16 Green IT
## Q56. Which of the following is an example of Green IT?
a) Development of a powerful in-house data center
b) Development of efficient in-house software
c) Using a desktop PC instead of a thin client laptop
d) Using web conferencing instead of traveling to meetings 

Answer: d) Using web conferencing instead of traveling to meetings

A / B / C / D format:

A ❌ → Powerful data centers usually increase energy consumption.
B ❌ → Software efficiency is good, but not directly related to reducing environmental impact in this context.
C ❌ → Desktop PCs typically consume more energy than thin clients/laptops.
D ✔ Green IT → Reduces travel, lowers fuel use and carbon emissions by replacing physical meetings with online conferencing

# 17 Chief Information Officer
## Q57. Which of the following is a major role of a CIO?
a) The CIO creates a plan to optimize the effect of investment on information resources
across the company to support business strategy when a computerization strategy is
established.
b) The CIO gives advice to the information system department by auditing whether the
information system functions properly in corporate activities.
c) The CIO receives queries about the information system, reports on the problems, and
gives specific instructions to the department in charge to ensure optimal management of
the company-wide information system.
d) The CIO understands the status of information system development and operation and
provides specific instructions on improvements to ensure that the company-wide
information system functions optimally. 

Answer: a) The CIO creates a plan to optimize the effect of investment on information resources across the company to support business strategy when a computerization strategy is established.

A / B / C / D format:

A ✔ CIO role → Strategic leadership: aligns IT investments with business strategy and optimizes information resources across the organization.
B ❌ → Describes auditing role (more like internal audit/IT auditor).
C ❌ → Operational instruction and troubleshooting (IT operations manager role).
D ❌ → Hands-on operational control and directives (not CIO-level strategic role).

Final Answer: A