# 1. AI Q3 
Q3. Which of the following is the most appropriate description of machine learning in AI?
a) It is a technology that enters specialized knowledge in a particular field into a computer,
and has the computer infer by using the knowledge entered.
b) It is a technology that gives computers the ability to learn in the same way humans
naturally learn, such as finding specific patterns from memorized data.
c) It is a technology that reproduces vital phenomena or evolutionary processes by using
computers and machines.
d) It is a technology to give computers the ability to manage learning materials and learning
by using a web system or other information technology so that people can learn interactively.

## Explination
a) Expert system / rule-based AI (uses predefined knowledge + inference rules)
b) Machine learning (computer learns patterns from data like humans learn from experience) ✅
c) Evolutionary computation / simulation (biological or evolutionary process modeling)
d) E-learning system (web-based learning management for humans)

# 2. Treee Traversal  
Q5. Among the four tree traversal techniques—breadth-first, in-order, post-order, and preorder—which of the following is the appropriate combination to ensure that the last two
nodes visited are the same in the tree shown below, when the left child is explored first? 
       18
      /  \
     5    20
    /      \
   3        22

a) Breadth-First Post-order
b) Breadth-First Pre-order
c) In-order Post-order
d) In-order Pre-order 

## Note 
Breadth-First -> level 
Post order -> Left Right Root
In order ->  Left Root Right
Pre order -> Root Left Right 

# 3. depth-verse traversal
Q6. In the graph shown below, which of the following is the output of a depth-first traversal
starting from vertex A, and visiting all vertices in ascending character order?  
   A       D ----- E
   |      / \
   |     /   \
   B --- C --- F

a) A B C D E F b) A B C D F E
c) A B D E F C d) A B D F E C

## Explaination
Traverse with ASC character

# 4. Q7 Hash Table
## Q7. Hash Table (Open Addressing with Linear Probing)

A hash table of size **11** uses open addressing with hash function:

h(k) = k mod 11

and **linear probing**.

The table shown below is created after inserting **4 values** into an initially empty hash table.

### Final Hash Table:

| Index | Value |
|------|------|
| 0    |      |
| 1    |      |
| 2    | 79   |
| 3    | 14   |
| 4    | 35   |
| 5    | 92   |
| 6    |      |
| 7    |      |
| 8    |      |
| 9    |      |
| 10   |      |

---

### Question:
Which of the following is the sequence that represents a possible order in which the key values were inserted into the table?

a) 14, 79, 35, 92  
b) 79, 14, 92, 35  
c) 79, 92, 35, 14  
d) 92, 79, 14, 35  

---

### Answer:
**a) 14, 79, 35, 92**

---

### Reasoning:

Hash values:
- 79 → 2
- 14 → 3
- 35 → 2 (collision)
- 92 → 4

Observations:
- 35 is at index 4 → must come after 79 and 14
- 92 is at index 5 → must come after 35

Thus valid order:
14 → 79 → 35 → 92

# 5. Q8 computer exe time calculation MIPS
## Q8. For a CPU with a clock frequency of 800 MHz, where one instruction is executed in an
average time of 4 clock cycles, what is the CPU performance in MIPS?
a) 0.2 b) 20 c) 200 d) 3,200 


want Total MIPS MIPS = num of instruction / number of exe time
KIPS = 10 power 3 instruction / sec
MIPS = 10 power 6 instruction / sec
GIPS = 10 power 9 instruction / sec

# 6. Q11 Cloud Computing
Q11. Which of the following is a merit of migrating an internal business system to a cloud
service?
a) If an internal business system that requires a very high level of availability is to be
migrated to IaaS, all service providers guarantee high availability, so the migration is
easy.
b) If an internal on-premises business system with company-specific functions is to be
migrated to a system provided by SaaS, the migration of the company-specific functions
also becomes easier.
c) If PaaS is to be used, platform management and OS updates are performed by the service
provider, so the burden of installation and operation can be reduced.
d) If SaaS is to be used temporarily for the development or evaluation of an internal
business system, a highly flexible development environment can be provided.


## IaaS (Infrastructure as a Service)
“You manage most things” → Long-term meaning:

High control & flexibility
Can build anything (custom systems, legacy apps)
BUT:
Ongoing maintenance burden
Need skilled engineers
More responsibility (security, updates, scaling)

👉 Best for: companies needing control or custom infrastructure
👉 Trade-off: flexibility ↑ but effort & cost of management ↑

## PaaS (Platform as a Service)
“Provider manages platform” → Long-term meaning:

You focus on development, not infrastructure
Faster development cycles
Less operational overhead

BUT:

Some vendor lock-in
Less control than IaaS

👉 Best for: long-term app development with efficiency
👉 Trade-off: productivity ↑, control ↓ (but usually worth it)

## SaaS (Software as a Service)
“Fixed software” → Long-term meaning:

Very easy to use & maintain
No need to build or manage anything
Scales easily

BUT:

Limited customization
Depends heavily on provider
Hard to fit unique business processes

👉 Best for: standard business needs (email, CRM, HR systems)
👉 Trade-off: convenience ↑, flexibility


## 🔥 Simple way to remember (long-term view)
IaaS → Freedom but responsibility
PaaS → Balance (most practical choice)
SaaS → Convenience but restrictions

## 🧠 Exam shortcut
If the question says:
“reduce burden” → PaaS ✅
“customization” → IaaS ✅
“standard service / easy use” → SaaS ✅
“flexibility” → usually NOT SaaS ❌

# 7 Q12 System Availability
Q12 In a system that is composed of two processing devices, what is the difference in
availability between the two conditions below? Here, the availability of each processing
device is 0.9, and no other factors besides the processing devices are considered.
[Conditions]
(1) The system is available if at least one of the processing devices is running normally.
(2) The system is available only if both of the processing devices are running normally.
a) 0.09 b) 0.10 c) 0.18 d) 0.19

✔️ Quick memory shortcut:
Parallel (OR condition) → use 1 − (fail × fail × …)
Series (AND condition) → use multiply directly
🔥 Super simple way to remember:
Parallel → backup exists → subtract failure
Series → no backup → multiply success


# 8 Q27 DNS cache Posining 
Q27. Which of the following is the attack that is classified as DNS cache poisoning?
a) False domain information is injected into the DNS server that is referenced by a PC, and
it leads the user to a fake server.
b) In order to interrupt the target service, the attacker uses the DNS server as a
steppingstone to send a large number of recursive queries.
c) In order to obtain internal information, the zone information stored in the DNS server is
compiled and transferred.
d) The version information of the DNS server software is obtained to identify a security
hole.

## EXPLANATION
Short explanations for each option:

a) (Correct – DNS cache poisoning)
This describes DNS cache poisoning.

Fake domain info is inserted into a DNS server’s cache
Users get redirected to a malicious (fake) website
👉 This is exactly what DNS cache poisoning does

b)
This is related to a DNS amplification attack

Uses DNS servers to flood a target with traffic
It’s a type of DDoS attack, not cache poisoning

c)
This is DNS zone transfer

Attacker copies DNS records from a server
Used for reconnaissance (getting internal info)

d)
This is DNS fingerprinting

Attacker checks DNS software version
Helps find vulnerabilities to exploit

Summary:

a = cache poisoning ✅
b = DDoS (amplification)
c = information gathering (zone transfer)
d = vulnerability scanning (fingerprinting)

#9 Q28 Database
Q28. A given application only has the functions of retrieving and displaying user information
from a database that stores such information. When considering information security, which
of the following is the appropriate database access right assigned to an account that the
application uses to access the database? The names and scopes of rights are listed below.
[The names and scopes of rights]
Reference right: Allows the application to select a record
Update right: Allows the application to insert, update, and drop a record
Administrator right: Allows the application to display, create, alter, and drop a
table
a) Administrator right b) Reference right
c) Update right d) Update right and reference right 

# 8 Q29 SaaS
Q29. Which of the following is a merit in using SaaS?
a) No system access management needs to be performed, and no consideration concerning
the procedure for password initialization or a password policy that satisfies complexity
requirements is required.
b) No system construction needs to be performed, and neither the definition of security
requirements for application software development nor the design of storage volume for
system logs is required.
c) No system operation needs to be performed, and no consideration concerning work
procedures at the time of a failure or backup is required.
d) No system security management needs to be performed, and neither the creation of
information security management rules nor the assignment of an administrator is
required. 

a) Access control still needed (passwords, users still managed)
b) ✔ No system build needed; provider handles security design & log storage
c) Operations/backup planning still partly required
d) Security management & admin roles still needed by customer

# 9 Secruity IC card and Pin 
Q30. Which of the following is an appropriate operation for user authentication that uses an
IC card and a PIN?
a) Given that each user can be identified by an IC card, a common PIN is set for all users in
order to reduce the management workload.
b) If an IC card is lost, a new IC card is issued, and after the PIN is reset, the lost IC card is
deactivated.
c) The PIN is set by combining the numeric information imprinted on the surface of the IC
card.
d) When an IC card is delivered, the PIN is not enclosed, but is notified to the user through
another channel. 

# 10 Check File Changes
Q31. Which of the following is the most effective method of detecting unauthorized changes of the contents of a web server?
a) Communications to the web server are monitored to ensure that there is no
communication other than HTTP and HTTPS.
b) The hash value of each file of the contents of the web server is stored and periodically
compared with the hash value generated from each file.
c) The memory usage of the web server is checked periodically to ensure that a buffer
overflow has not occurred.
d) The updated date of each file of the contents of the web server is stored and compared
periodically with the updated date of each file. 

## Explanation
a) ❌ Wrong
Monitoring HTTP/HTTPS traffic does not detect file tampering inside the server
b) ✔ Correct
File hash values are stored and periodically compared → detects any unauthorized modification accurately
c) ❌ Wrong
Memory usage check does not directly detect content changes on web files
d) ❌ Wrong
File timestamps can be easily changed → not reliable for detecting tampering

# 11 WAF firewall
Q32. Which of the following is the function of a WAF?
a) Encrypting data and controlling access on web server
b) Inspecting and filtering HTTP requests
c) Managing user authentication and authorization
d) Scanning malware on a web server

## Explanation
a) ❌ Wrong
WAF does not encrypt data or manage access control
b) ✔ Correct
WAF (Web Application Firewall) inspects and filters HTTP/HTTPS requests to block attacks like SQL injection, XSS
c) ❌ Wrong
Authentication/authorization is handled by application systems, not WAF
d) ❌ Wrong
Malware scanning is done by antivirus or security tools, not WAF

✔ Final: b (WAF = filters and monitors web traffic requests)

# 12 SPF ( mail check like WAF )
Q32. Which of the following is the function of a WAF?
a) Encrypting data and controlling access on web server
b) Inspecting and filtering HTTP requests
c) Managing user authentication and authorization
d) Scanning malware on a web server

a) ❌ Wrong
WAF does not handle encryption or access control
b) ✔ Correct
WAF (Web Application Firewall) inspects and filters HTTP/HTTPS requests to block attacks like SQL injection and XSS
c) ❌ Wrong
Authentication and authorization are handled by the application or identity systems
d) ❌ Wrong
Malware scanning is done by antivirus/security software, not WAF

✔ Final: b (WAF = filters web traffic at application layer)

# 13 resource allocation
Q46. Which of the following is a technique that is used to perform the optimal resource allocation for a computerization investment in each category classified on the basis of the similarities in risks and investment value?
a) 3C analysis b) Benchmarking
c) Enterprise architecture d) IT portfolio

## Explanation
Short notes:

a) ❌ 3C analysis
Used for market analysis (Company, Customer, Competitor), not IT investment allocation
b) ❌ Benchmarking
Comparing performance with others, not resource allocation method
c) ❌ Enterprise architecture
Framework for aligning IT with business structure, not allocation technique
d) ✔ IT portfolio
Used to classify and manage IT investments based on risk and value for optimal resource allocation

✔ Final: d (IT portfolio = prioritizing and allocating IT investments effectively)

# 14 UML For data daigram

Q47. Which of the following is a usage scenario for the adoption of UML as a technique for
visualizing business processes?
a) Diagrams are shown by using a data-oriented approach where objects are handled as
entities, their attributes, and the relationships among the entities.
b) To represent processes by using data flows, sources and sinks of data, data stores, and
data processes are connected with arrows that indicate data flow.
c) To represent processes from multiple viewpoints, some purpose-specific modeling
methods are used, and each model is depicted by using standardized notation rules for
object modeling.
d) To thoroughly represent the functions of a process, the events that occur in response to a
single request are described by using the conditional branch format. 

## Explanation
Short notes:
a) ❌ Wrong
Describes ER (Entity-Relationship) style modeling, not UML usage scenario

b) ❌ Wrong
This is DFD (Data Flow Diagram) approach, not UML

c) ✔ Correct
UML is used to model systems from multiple viewpoints using standardized object-oriented diagrams (class, use case, sequence, etc.)

d) ❌ Wrong
Describes flow/branch logic like activity or flowchart style, not UML purpose as a whole

✔ Final: c (UML = standardized multi-view object-oriented modeling)

# 15 Hybrid Cloud
Q48. Which of the following is an explanation of a hybrid cloud?
a) To configure and provide the service content of a cloud service for both consumers and
companies
b) To customize some of the functions that are provided by a cloud service for the
company’s own use
c) To provide an environment where data and application software are linked and
interoperable between a cloud service for the exclusive use of a company and a generalpurpose cloud service
d) To separately provide the service content of a cloud service as paid services and free
services 

## Explanation
Short notes:

a) ❌ Wrong
Describes general cloud service usage, not hybrid cloud
b) ❌ Wrong
Talks about customization, not cloud integration type
c) ✔ Correct
Hybrid cloud = integration between private (company-only) cloud and public (general-purpose) cloud with interoperability
d) ❌ Wrong
Describes pricing model (free vs paid), not architecture

✔ Final: c (Hybrid cloud = private + public cloud working together)


# 16 Green procurement
Q49. Which of the following is an explanation of green procurement?
a) It refers not only to the fulfillment of the requirements of quality and price but to the
preferential purchase of products and services with a lower environmental burden from
companies that work toward a reduction in their environmental impact.
b) It refers to a certificate that enables commercial trading of the green power that is
generated from natural energy sources such as solar, biomass, wind power, and
geothermal heat.
c) It refers to international standards concerning environmental labels that are certified by a
third party on the basis of certain criteria.
d) It refers to mass promotion of the details of environmental protection activities and
raising funds for environmental protection from investors. 

## Explanation
Short notes:

a) ✔ Correct
Green procurement = buying products/services based on low environmental impact + supplier’s eco-friendly practices
b) ❌ Wrong
Describes green power certificate / renewable energy trading
c) ❌ Wrong
Describes eco-label certification standards (ISO-type labeling systems)
d) ❌ Wrong
Describes environmental fundraising / awareness activities

✔ Final: a (green procurement = environmentally conscious purchasing)