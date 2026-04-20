# 1.Q5 Tree traversals
DFS → explore deep paths first
BFS → explore wide/level first

## 1. Depth-First Traversals (DFS)
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

## Breadth-First Traversal (BFS)
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

## Tree Traversals in E-commerce

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


# 2.Q6 Flowchart 
-------------------------------------------------------------------------------------------------------------------------------------------------------------
The flowchart below shows an algorithm that determines the sum (i.e. “1 +3+ 5+ … +(2N-1)”) of the first N odd integers from 1 through 2N-1 (where N ≥ 1) and inserts the result into variable x. Which of the following is an expression to be inserted in blank A ? 


N = odd int
N odd integers
2N01 ( where N>/ 1 )
x= the final result
A = ?


# 3.Q7 Bubble Sort
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



# 4.Q11 Foolproof
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


# 5.Q15 Hashing
-------------------------------------------------------------------------------------------------------------------------------------------------------------

  ## 🔑 What is Hashing?

  Hashing is the process of taking an input (like a word, file, or password) and running it through a hash function to produce a fixed-length output called a hash value (or digest).

  Input: "hello"
  Output (example hash): 5d41402abc4b2a76b9719d911017c592

  Even a tiny change in input (like "Hello" vs "hello") produces a completely different hash.

  ## ⚙️ How It Works

  A hash function:

  Takes input of any size
  Produces output of fixed size
  Is deterministic (same input → same output)
  Is fast to compute

  Good hash functions also:

  Minimize collisions (different inputs giving same output)
  Spread values evenly
  📦 Common Uses of Hashing
  ## 1. 🔍 Data Structures (Hash Tables)

  Hashing is used in structures like hash tables (e.g., dictionaries in Python).

  Key → hash → index → value
  Makes lookups very fast (O(1) average time)
  Hash Table (in memory, fast lookup)
  Key        →   Hash Function   →   Index   →   Value
  ----------------------------------------------------
  "user1"    →      ####         →    [3]    →  Alice
  "user2"    →      ####         →    [7]    →  Bob
  "user3"    →      ####         →    [1]    →  Charlie


  Internal Array (Hash Table):
  Index:   0    1       2    3       4    5    6    7
          [ ] [Charlie] [ ] [Alice] [ ] [ ] [ ] [Bob]

  ## 2. 🔐 Password Storage

  Instead of storing passwords directly, systems store their hashes.

  User enters password → hashed → compared with stored hash
  Even if data is stolen, original passwords aren’t easily revealed

  Popular hash algorithms:

  MD5 (old, not secure)
  SHA-1 (deprecated)
  SHA-256 (secure)

  You type password:

  "123456"

  System hashes it again:

  hash("123456") → "abcdef"

  Compare with stored value:

  "abcdef" == "abcdef" ✅

  👉 It never “decrypts” anything

  ## 3. 📁 Data Integrity (Checksums)

  Used to verify files haven’t been altered.

  Download file → compute hash → compare with original hash

  👉 Very short note:

  Owner provides: hash algorithm + hash value
  Downloader computes hash of file
  Compare both

  👉 Same → ✅ file intact
  👉 Different → ❌ file changed

  ## 4. 🌐 Cryptography

  Hashing is used in:

  Digital signatures
  Blockchain systems (like Bitcoin)
  Message authentication


# 6.Q17 Animation Motion
##  Keyframe Method

👉 Manual animation technique

Animator sets important frames (start, end)
Computer fills in the movement between them

🧠 Think:

“Draw main poses → computer fills gaps”

## Morphing

👉 Transform one image/object into another

Smoothly changes shape
Often used in effects

🧠 Think:

“Face → slowly turns into another face”

## Motion Capture ✅ (Correct answer)

👉 Records real movement using sensors & cameras

Captures human/animal motion
Converts it into animation data

🧠 Think:

“Real movement → digital animation”

## Pixel Shader

👉 Graphics processing (NOT animation recording)

Controls how pixels look (color, lighting, effects)
Runs on GPU

🧠 Think:

“Makes things look realistic (lighting, shadows)”

✅ Final Answer:

## Motion capture

🧠 Super quick memory trick
Keyframe → manual animation
Morphing → shape change
Motion capture → real movement recording ⭐
Pixel shader → visual effects


# 7.Q27 Security
## Which of the following describes a brute force attack aimed at finding the key of
symmetric encryption?
a) Finding the key by observing the ciphertext change when the plaintext is altered by a
certain amount
b) Finding the key by testing all key combinations sequentially when a set of plaintext and
ciphertext is given
c) Finding the key by using the algebraic expression representing the relationship between
the plaintext, ciphertext, and key as a clue
d) Finding the key by using the statistical correlation between a part of the information of
the plaintext and part of the information of the ciphertext as a clue 

## Key Concepts
Symmetric Encryption:
Encryption where the same key is used to encrypt and decrypt data.
Example: AES, DES.
Plaintext:
Original readable data/message before encryption.
Ciphertext:
Encrypted data (scrambled, unreadable without the key).
Ciphertext Change / Observing differences:
When you change the plaintext and look at how ciphertext changes — used in differential attacks, not brute force.

## Difference from brute force:
An algebraic attack targets weaknesses in the mathematical structure of the encryption algorithm itself instead of just trying keys blindly.

Brute force: Try every key sequentially.
Algebraic: Use math relationships to shortcut the search for the key. ( # the weaknes of the encryption method by mathamatically)

# 8.Q28 Security
## Which of the following is a package of unauthorized programs and tools that has
functions such as creating a backdoor on a server and hiding the evidence of intrusion inside
the server?
a) RFID b) Rootkit c) TKIP d) Web beacon 

## a) RFID (Radio Frequency Identification)
A technology that uses radio waves to identify and track objects (like ID cards, key cards, or inventory tags) without needing direct contact. ( wireless track credit card casher etc..)
## b) Rootkit
A type of malicious software designed to secretly gain control of a computer and hide its presence, often giving hackers deep access to the system. hacker sofs
## c) TKIP (Temporal Key Integrity Protocol) 
A security protocol used in older Wi-Fi networks (like WPA) to encrypt data and protect wireless communication, now mostly replaced by stronger methods. ( not physical device its just encryption methods )

## d) Web beacon
A tiny invisible image or piece of code on a webpage or email used to track user behavior (like whether you opened an email or visited a page).

## so the answer is Rootkit


# 9.Q28 Encryption Algorythhm

Q)Which of the following is a public-key cryptography algorithm whose security depends
on the difficulty of factoring extremely large numbers into primes?

## 🔐 Encryption algorithms

  a) Symmetric (like AES)
  One key
  Encrypt + decrypt
  Used for securing data

  b) Asymmetric (public/private key)
  RSA → encryption + signatures
  Diffie–Hellman → sharing keys securely
  DSA → digital signatures

## a) AES (Advanced Encryption Standard)

  A fast and secure encryption method used to protect data (like passwords, files, Wi-Fi). It uses the same key to encrypt and decrypt.
            AES	                              SHA/Hash
  Symmetric encryption (reversible)	  One-way hash (irreversible)
  Can decrypt if you have the key	    Cannot get original password from hash
  Used to secure files, messages	    Used to store passwords safely

## b) DH (Diffie-Hellman)
  A method that lets two parties securely share a secret key over the internet, even if others are watching.

  A method where two parties use a standard public formula and exchange public values to generate the same secret key, 
  without sharing their private numbers or the secret key.

  ^ is same with power

  Public:
  g^a mod p, g^b mod p

  Secret:
  g^(ab) mod p

  Real Wold use case 

🌐 1. HTTPS (secure websites)

    When you open:

    banking sites
    Gmail
    online shopping

    👉 Your browser and the server use Diffie-Hellman to:

    securely agree on a shared encryption key
    even if hackers are watching the network

    Then they use that key to encrypt all data (passwords, cards, messages).
    .

📱 2. Messaging apps (Signal, WhatsApp, Telegram)

    Apps use Diffie-Hellman (or variants like ECDH) to:

    create a shared secret key
    enable end-to-end encryption

    👉 Only sender and receiver can read messages.

🔐 3. VPN connections

    When you connect to a VPN:

    Diffie-Hellman helps your device + VPN server agree on a secret key
    used to encrypt all your internet traffic


## c) DSA (Digital Signature Algorithm)
A technique used to verify that a message is authentic and hasn’t been changed (digital signatures).
Real-world use cases of DSA
Signing (by sender):

Message + private key → digital signature

Verification (by receiver):

Message + signature + public key → “valid” or “invalid”

Key idea
Private key = proves “I wrote this”
Public key = lets others confirm “Yes, it’s really you”

1. Software update verification

Companies sign software updates so users can confirm the file is genuine.
When you download an app update, the system checks the digital signature before installing it.
This helps prevent malware disguised as official updates.

2. Secure email and documents

Sensitive documents (like contracts or government forms) can be digitally signed.
The recipient can verify who sent it and that it wasn’t changed after signing.

3. Git and code integrity (development)

Developers can sign commits using tools like GPG.
This ensures the code really came from the claimed developer and wasn’t tampered with in the repository history.

4. Secure communication systems (SSH/TLS historically)

DSA has been used in secure login systems like SSH for authentication.
It helps verify the identity of a server or user during secure connections.

5. Government and legal systems

Used in some e-governance systems for signing digital records, tax filings, and legal approvals.
Ensures accountability and prevents forgery.
Simple idea

DSA acts like a tamper-proof digital stamp + signature combined:

Signature = proves identity
Tamper check = proves data hasn’t changed

If you want, I can also show a step-by-step example of how a DSA signature is created and verified.


## d) RSA (Rivest–Shamir–Adleman)
A widely used encryption system that uses two keys (public + private) for secure communication and digital signatures.

  🔐 What is RSA?

  RSA (Rivest–Shamir–Adleman) is a public-key cryptography system used for:

  Encrypting data (privacy)
  Creating digital signatures (authenticity)
  Secure key exchange

  It uses two keys:

  🔑 Public key → shared with everyone
  🔒 Private key → kept secret
  🧠 Simple idea
  Public key = “lock”
  Private key = “key to open the lock”

  Anyone can lock (encrypt) a message, but only the owner can unlock it.

  🌍 Real-world use cases of RSA
  1. 🌐 HTTPS (secure websites)
  When you see a 🔒 padlock in your browser
  RSA helps your browser securely connect to websites (like Google, banking sites)
  Protects passwords and personal data
  2. 📧 Email security
  Used in secure email systems (like PGP)
  Ensures:
  Only the right person reads the email (encryption)
  Email is not changed (signature)
  3. 🔐 Digital signatures
  Used to verify software, apps, and documents
  Example:
  Windows/macOS updates are signed so you know they are real
  Prevents malware pretending to be official software
  4. 🔑 Secure login systems (SSH / VPN)
  Used when logging into servers remotely (SSH)
  Helps verify identity without sending passwords openly
  5. 🏦 Banking & online payments
  Protects sensitive communication between:
  banks
  payment gateways
  credit card systems
  ⚡ Why RSA is important
  Ensures privacy (encryption)
  Ensures trust (authentication)
  Ensures data integrity (no tampering)
  🧩 One-line summary

  RSA is the system that helps make the internet secure, trusted, and private using public and private keys.

| Feature              | DSA                                                 | RSA                         |
| -------------------- | --------------------------------------------------- | --------------------------- |
| Purpose              | Only digital signatures                             | Encryption + signatures     |
| Key types            | Private + Public keys                               | Private + Public keys       |
| Speed (signing)      | Fast                                                | Slower                      |
| Speed (verification) | Slower than RSA                                     | Fast                        |
| Security basis       | Discrete logarithm problem                          | Prime factorization problem |
| Common use today     | Less common now (replaced by ECDSA in many systems) | Still widely used           |



🔑 One key (symmetric encryption):

AES → uses 1 same key for both encryption and decryption

🔐 Two keys (asymmetric encryption):


✍️ Digital signature (uses key pairs):

DSA → uses 2 keys (public + private) for signing and verification


RSA → uses 2 keys (public + private)

🤝 Key exchange method (not exactly encryption):

DH (Diffie-Hellman) → used to create/share a key, not to encrypt data itself


✅ Summary:

AES → 1 key
RSA, DSA → 2 keys
DH → key exchange (helps create keys)

| Feature      | Symmetric (AES)      | Asymmetric (RSA/DSA)      |
| ------------ | -------------------- | ------------------------- |
| Keys         | 1 shared key         | 2 keys (public + private) |
| Speed        | Fast ⚡               | Slower 🐢                 |
| Security use | Bulk data encryption | Key exchange, signatures  |
| Examples     | AES                  | RSA, DSA                  |




# 10.Q30 Security ( Attacking Poisoning) 

## Attacking 

Which of the following is the name of an attack where manipulation is employed to place
a malicious website near the top of the search results on a search engine?

## a) Cross-site scripting 
  It happens when an attacker injects malicious scripts (usually JavaScript) into a trusted website. These scripts then run in other users’ browsers when they visit the site.

  Key idea: the website unknowingly “trusts” and displays harmful code.

  What attackers can do:

  Steal cookies or login sessions
  Redirect users to fake sites
  Deface web pages or change content
  Perform actions as the user without permission

  Common types:

  Stored XSS: malicious script is saved on the server (e.g., in comments)
  Reflected XSS: script comes from a request and is immediately shown back
  DOM-based XSS: happens in the browser due to unsafe JavaScript handling

  Prevention:

  Validate and sanitize user input
  Escape output properly in webpages
  Use security headers like Content Security Policy (CSP)

  In short, XSS is when a website accidentally allows attackers to run harmful scripts in other users’ browsers.

## b) DNS cache poisoning
  DNS Cache Poisoning (also called DNS spoofing) is a type of cyber attack where fake or incorrect information is inserted into a DNS resolver’s cache.

  DNS (Domain Name System) is what translates website names (like google.com) into IP addresses. When the cache is “poisoned,” it gives users the wrong IP address.

  What happens in the attack:

  A user types a real website name
  The DNS server returns a fake IP address (from attacker)
  The user is redirected to a malicious website without knowing

  Effects:

  Stealing login credentials
  Redirecting users to fake or phishing sites
  Spreading malware

  Prevention methods:

  Use DNSSEC (Domain Name System Security Extensions)
  Keep DNS servers updated and secured
  Clear and protect DNS cache regularly
  Use trusted DNS providers

  In short: DNS cache poisoning tricks a DNS server into giving wrong website addresses, sending users to fake or harmful sites.

## c) SEO poisoning
  SEO Poisoning (Search Engine Optimization poisoning) is a cyber attack where attackers manipulate search engine results so that malicious or fake websites appear at the top of search results.

  How it works:

  Attackers create harmful or fake websites
  They use SEO techniques (keywords, backlinks, trending topics) to rank higher
  Users searching for something normal click on these top results
  They are then redirected to phishing pages or malware sites

  Effects:

  Stealing personal information (passwords, banking details)
  Installing malware or spyware on devices
  Spreading scams or fake downloads

  Common targets:

  Popular search terms (movies, software downloads, news, free tools)

  Prevention:

  Be careful clicking top search results, especially ads or unknown sites
  Use trusted websites directly instead of searching every time
  Keep antivirus and browsers updated
  Check URLs before entering sensitive information

  In short: SEO poisoning is when attackers “trick search engines” so harmful websites appear as trusted search results.

## d) Social engineering 
  Social Engineering is a cyber attack technique where attackers manipulate people into revealing confidential information or performing unsafe actions, instead of hacking systems directly.

  How it works:
  Attackers use trust, fear, curiosity, or urgency to trick individuals into giving away sensitive data like passwords, OTPs, or personal details.

  Common methods:

  Phishing emails or messages
  Pretending to be bank staff, tech support, or trusted companies
  Fake phone calls or websites
  Baiting (offering fake rewards or downloads)

  Effects:

  Identity theft
  Financial loss
  Unauthorized access to accounts or systems

  Prevention:

  Do not share passwords or OTPs with anyone
  Verify identity before trusting requests
  Be cautious of urgent or suspicious messages
  Use two-factor authentication (2FA)

  In short: Social engineering is tricking people, not computers, to gain unauthorized access to information.



# 11.Q31 Security (timestamp service in information security)
## Which of the following is an explanation of the ? 
## a)It is a service that authenticates biometric information, such as fingerprints, voice prints,vein patterns, retina, and iris, by using the date and time when the information is registered in the authentication system.

  This service checks a person’s identity using biometric data like:

  fingerprint
  iris/retina scan
  voice pattern
  vein pattern

  What makes it special is that it also records the exact date and time when the biometric data was registered or used.

  👉 So it not only says “this is you”, but also “this identity was confirmed at this specific time.”

## b) It is a service that certifies that electronic data certainly exists on a particular date and
  time and that the data has not been modified since that date and time.

  This service proves two things about electronic data:

  The data existed at a specific date and time
  The data has not been changed since then

  👉 Example: If you create a document today, this service can prove later that:

  “This file existed on April 11 and hasn’t been modified.”

  It is often used for legal proof, contracts, and digital signatures.


## c) It is a service that securely verifies that the date and time information is not falsified
  midway for setting the clocks of the PCs and servers on the network.

  This service ensures that the time on computers and servers is correct and not tampered with.
  Normally, devices set their clocks using internet time, but attackers could try to change that.
  👉 This service protects against fake time updates and ensures:
  PCs and servers all use the correct trusted time
  The time cannot be secretly altered It’s basically a secure version of network time syncing.

## d) It is a web service that securely displays the global date and time information used in
  official records by using encrypted communication. 
  This is a service that provides the official correct world time (like UTC) over a secure connection.
  It:
  Shows trusted global date/time
  Uses encryption so no one can alter the information in transit

  👉 Think of it as a secure official clock for systems and records worldwide.




# 12.Q32 Security ( improve an organization’s security posture )
  ## Which of the following is an appropriate term for an organized and highly skilled teamwhose mission is to continuously monitor and improve an organization’s security posture while preventing, detecting, analyzing, and responding to cybersecurity incidents, utilizing
  both technology and well-defined processes and procedures?

  ## a) Cybersecurity
  The practice of protecting computers, networks, and data from attacks, damage, or unauthorized access.

  ## b) Incident Management Center (IMC)
  A team or facility that handles and coordinates response to IT incidents or disruptions to restore normal service quickly.

  ## c) Network Operations Center (NOC)
  A center that monitors and manages an organization’s network infrastructure to ensure systems are running smoothly and efficiently.

  ## d) Security Operations Center (SOC)
  A team that continuously monitors, detects, analyzes, and responds to cybersecurity threats and security incidents.

# 13.Q33 Security ( octal value from 0 through 7 one bit is allocated for each of these three (3) permissions)

  ## Q In an OS where permissions for reading, writing, or executing a file can be independently set as attributes of the file, one bit is allocated for each of these three (3) permissions to determine whether they are allowed or not. When these three bits are configured using an octal value from 0 through 7, the trial results below are obtained. Which of the following is an appropriate trial result? 

    [Trial results]
    (1) When 0 is set, reading, writing, and execution can no longer be performed.
    (2) When 3 is set, reading and writing can be performed, but execution cannot.
    (3) When 7 is set, reading, writing, and execution can be performed. 

    a) When 2 is set, reading and execution can be performed.
    b) When 4 is set, only execution can be performed.
    c) When 5 is set, only writing can be performed.
    d) When 6 is set, reading and writing can be performed. 

    | Octal | Binary | Permissions | Meaning                                        |
    | ----- | ------ | ----------- | ---------------------------------------------- |
    | **0** | 000    | ---         | No permission (cannot read, write, or execute) |
    | **1** | 001    | --x         | Execute only                                   |
    | **2** | 010    | -w-         | Write only                                     |
    | **3** | 011    | -wx         | Write + execute                                |
    | **4** | 100    | r--         | Read only                                      |
    | **5** | 101    | r-x         | Read + execute                                 |
    | **6** | 110    | rw-         | Read + write                                   |
    | **7** | 111    | rwx         | Read + write + execute                         |


# 14.Q48 Stretagy ( Which of the following is an appropriate description of an RFI? () 

  ## a) SRS / System Requirements Specification (or Basic system requirement document)
  Describes system overview, purpose, functions, requirements, and constraints
  It is the core requirement document
  ✔ Basically: “What the system should do”
  ## b) RFP response / Proposal document
  A document created after an RFP is issued
  Vendors submit this to propose their solution
  ✔ Basically: “We can build it like this”
  ## c) RFP (Request for Proposal)
  Used by companies to ask vendors for detailed system proposals
  Includes requirements and expectations
  ✔ Basically: “Please propose how you will build this system”
  ## d) RFI (Request for Information)
  Used to collect basic information from vendors
  Before RFP stage
  ✔ Basically: “Tell us what solutions you offer”

  a) It is a document describing the basic policy for the system, including a summary of the
  system, purpose, necessary functions, system requirements, and contract matters.
  b) It is a document that is created after an RFP.
  c) It is a document used by companies looking for the implementation of computerization
  to request specific system proposals from prospective suppliers such as system vendors.
  d) It is a document used to request information concerning computerization from
  prospective suppliers such as system vendors

  ⚡ Super simple memory trick
  RFI = Ask information
  RFP = Ask for proposal
  Proposal = Vendor response
  SRS = Final system agreement

  RFI → RFP → Proposal → Contract/SRS → System Development

  🔵 Step 1: RFI (Request for Information)

📄 “We are planning a system. Tell us what you can offer.”

The school sends RFI to vendors like:

software companies
IT firms

👉 Vendors reply with:

what systems they have
technologies used
general capabilities

✔ Purpose: just gathering information

🟡 Step 2: RFP (Request for Proposal)

📄 “Now we want detailed solutions and pricing.”

The school sends RFP saying:

we need attendance + grading system
must support 5000 students
must be web-based

👉 Vendors reply with:

full system design
timeline
cost
technical plan

✔ Purpose: compare solutions and choose best vendor


# 15.Q53 Computer ( Knowledge) 
Which of the following is an appropriate computing concept that describes the idea of physical objects, such as devices, vehicles, and buildings, that are connected to the Internet and are able to identify themselves to other devices?

  ## a) Computer networks 
  A computer network is a system where multiple computers are connected to share resources and information. These connections can be wired or wireless. Networks allow communication through devices like routers and switches. Examples include LAN (Local Area Network) and the Internet.
  ## b) Deep learning
  Deep learning is a branch of machine learning that uses artificial neural networks with many layers. It helps computers learn patterns from large amounts of data. It is widely used in image recognition, speech recognition, and self-driving cars.
  ## c) Internet of things 
  The Internet of Things (IoT) refers to everyday physical devices connected to the internet. These devices collect and share data automatically. Examples include smart watches, smart homes, and connected cars.
  ## d) Network topology
  Network topology describes how devices in a network are arranged and connected. Common types include star, bus, ring, and mesh topologies. It affects network performance, reliability, and scalability.