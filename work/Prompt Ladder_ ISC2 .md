# **Prompt Ladder: ISC2 Cybersecurity Study**

**Module Task:** Study a module from my ISC2 course for my certificate in cybersecurity.  
**Methodology Note:** This document tracks the iteration of a prompt. Model comparisons are available in the final analysis section.

## **Baseline (V0)**

### **Prompt**

`Write some practice questions for the ISC2 CC exam.`

### **Output Excerpt**

#### **Claude:**

"Happy to help with both. Let's knock out the ISC2 CC practice questions first, then move into the portfolio interview. ISC2 CC (Certified in Cybersecurity) Practice Questions 1\. Which security principle ensures that data has not been altered by an unauthorized party? A) Confidentiality B) Integrity C) Availability D) Non-repudiation Answer: B 2\. A company implements a policy where employees only get access to the systems required for their specific job function. This is an example of: A) Separation of duties B) Least privilege C) Defense in depth D) Zero trust Answer: B 3\. Which type of attack involves an attacker intercepting communication between two parties without their knowledge? A) Phishing B) Man-in-the-middle C) Denial of service D) SQL injection Answer: B 4\. In the CIA triad, "Availability" is best described as: A) Ensuring only authorized users can view data B) Ensuring data is accurate and unaltered C) Ensuring systems and data are accessible when needed D) Ensuring actions can be traced to a specific user Answer: C 5\. A Disaster Recovery Plan (DRP) primarily focuses on: A) Preventing incidents from occurring B) Restoring IT systems and data after a disruptive event C) Communicating with the public during a crisis D) Training employees on security awareness Answer: B 6\. Which access control model assigns permissions based on a user's role within an organization? A) DAC (Discretionary Access Control) B) MAC (Mandatory Access Control) C) RBAC (Role-Based Access Control) D) ABAC (Attribute-Based Access Control) Answer: C 7\. A firewall that filters traffic based only on source/destination IP, port, and protocol, without tracking connection state, is called a: A) Stateful firewall B) Packet-filtering firewall C) Application firewall D) Next-gen firewall Answer: B 8\. What is the primary purpose of a Business Continuity Plan (BCP)? A) To recover data after a breach B) To ensure critical business functions continue during and after a disruption C) To document network topology D) To manage patch deployment schedules Answer: B 9\. Which of the following best describes "defense in depth"? A) Using a single, very strong security control B) Layering multiple security controls so if one fails, others still protect the asset C) Outsourcing all security functions to a third party D) Relying solely on perimeter firewalls Answer: B 10\. During the incident response process, which phase involves determining the root cause and removing the threat from the environment? A) Detection B) Containment C) Eradication D) Recovery Answer: C Want a second batch focused on a specific weak domain, or is this enough to start? Now — Portfolio Case Studies, Project \#1 Let's build your first case study. I'll ask one question at a time. Question 1: What's the project? Give me the name and a one-line description of what it is/does."

### **Notes**

| Category | Details |
| :---- | :---- |
| **What changed in the prompt** | N/A. |
| **What improved in the output** | N/A. |
| **What still failed** | Claude included unrelated content about a portfolio interview. The practice questions covered broad, generalized topics rather than focusing on a specific area of weakness. |
| **What to try next** | Add a role assignment to establish a professional persona and focus the AI on a specific instructional standard. |

## **Version 1 (+ Role Assignment)**

### **Prompt**

`Act as an expert cybersecurity instructor who specializes in preparing students for the ISC2 Certified in Cybersecurity (CC) exam.`  
`Write some practice questions for the ISC2 CC exam.`

### **Output Excerpt**

#### **Claude:**

"I'll help with both, but let's keep them separate and do one at a time cleanly — mixing a portfolio interview with an exam-prep request in the same thread will make the case-study interview harder to follow later. Let's knock out the CC practice questions first since that's a quick, self-contained task, then move into the project interview. ISC2 CC Practice Questions Domain 1: Security Principles Which of the following best describes the concept of "least privilege"? a) Users are granted the minimum access necessary to perform their job functions b) All users share a common set of default permissions c) Access is granted based on seniority within the organization d) Administrators have unrestricted access to all systems The CIA triad consists of Confidentiality, Integrity, and Availability. Which scenario represents a violation of integrity? a) A DDoS attack takes a website offline b) An unauthorized user reads sensitive customer data c) An attacker modifies financial records without authorization d) An employee loses their encrypted laptop Domain 2: Business Continuity, Disaster Recovery & Incident Response What is the primary difference between a Business Continuity Plan (BCP) and a Disaster Recovery Plan (DRP)? a) BCP focuses on IT systems only; DRP focuses on all business operations b) BCP ensures overall business operations continue; DRP focuses specifically on restoring IT infrastructure c) They are interchangeable terms for the same plan d) DRP is only used for natural disasters During an incident response, which phase involves determining the root cause and removing the threat from the environment? a) Detection b) Containment c) Eradication d) Recovery Domain 3: Access Control Concepts Which access control model assigns permissions based on a user's role within an organization? a) Discretionary Access Control (DAC) b) Mandatory Access Control (MAC) c) Role-Based Access Control (RBAC) d) Rule-Based Access Control What is "something you have" an example of in multi-factor authentication? a) A password b) A fingerprint c) A hardware token d) A security question Domain 4: Network Security Which device operates primarily at Layer 3 of the OSI model to route traffic between different networks? a) Switch b) Router c) Hub d) Repeater A VPN primarily provides which security benefit when accessing a network remotely? a) Malware scanning b) Encrypted tunnel for data in transit c) Physical access control d) Patch management Domain 5: Security Operations What is the main purpose of a Security Information and Event Management (SIEM) system? a) To physically secure server rooms b) To aggregate and analyze log data for threat detection c) To encrypt data at rest d) To manage user password resets Which type of security control is a firewall considered? a) Administrative b) Physical c) Technical d) Corrective Answer Key: 1-a, 2-c, 3-b, 4-c, 5-c, 6-c, 7-b, 8-b, 9-b, 10-c Want me to generate more (I can weight them toward domains you're weaker on), or convert these into a formatted document/artifact you can drill from? Now, switching hats — let's get into Week 2: Case Studies. I'll interview you one project at a time. Give me the name of the first project you want to feature, and a one-line description of what it is.”

### **Notes**

| Category | Details |
| :---- | :---- |
| **What changed in the prompt** | Added the role of an expert cybersecurity instructor to ground the AI's vocabulary and expertise. |
| **What improved in the output** | Claude organized the 10 questions systematically by their specific exam domains. |
| **What still failed** | Claude continued to include the unrelated portfolio interview text at the end of its response. The output still provided generalized questions across all domains instead of targeting a specific focus area. |
| **What to try next** | Provide context and motivation to explicitly instruct the AI to focus on a single, specific area of weakness. |

## **Version 2 (+ Context and Motivation)**

### **Prompt**

`Act as an expert cybersecurity instructor who specializes in preparing students for the ISC2 Certified in Cybersecurity (CC) exam.`  
`I am an Information Systems student taking the ISC2 CC exam soon to transition into the cybersecurity field. I am struggling with Domain 4: Network Security, specifically concerning the OSI model and secure protocols. I need to test my knowledge to identify my blind spots so I don't fail the real exam.`  
`Write some practice questions for the ISC2 CC exam.`

### **Output Excerpt**

#### **Claude:**

"It looks like two different briefs got pasted into one message — the portfolio copywriting coach setup and the ISC2 CC exam prep request. I'll run with the cybersecurity request since that's what you're asking me to act on right now. If you want to start the portfolio interview afterward, just say so and we'll kick off Week 2\. Here are 10 practice questions covering OSI model and secure protocols (ISC2 CC, Domain 4). Try answering all of them first — then check the answer key below so you get an honest read on your blind spots rather than second-guessing as you go. 1\. At which OSI layer does a switch primarily operate when forwarding frames based on MAC addresses? A) Layer 1 – Physical B) Layer 2 – Data Link C) Layer 3 – Network D) Layer 4 – Transport 2\. Which protocol is responsible for resolving a domain name to an IP address? A) DHCP B) ARP C) DNS D) SNMP 3\. A network engineer wants to encrypt traffic between two branch offices over the internet. Which technology is most appropriate? A) VLAN B) VPN C) NAT D) Proxy server 4\. Which OSI layer is responsible for establishing, maintaining, and terminating sessions between applications? A) Layer 4 – Transport B) Layer 5 – Session C) Layer 6 – Presentation D) Layer 7 – Application 5\. Which of the following protocols provides secure remote command-line access, replacing an older insecure equivalent? A) Telnet B) SSH C) FTP D) HTTP 6\. TLS primarily operates to secure communications at which point in the network stack? A) Strictly at Layer 3 B) Between the Transport and Application layers C) Only at Layer 1 D) Within the Data Link layer only 7\. Which protocol should replace FTP when file transfer confidentiality and integrity are required? A) TFTP B) SFTP C) SMTP D) ICMP 8\. A device converts digital data into electrical, radio, or optical signals for transmission. This function belongs to which OSI layer? A) Layer 1 – Physical B) Layer 2 – Data Link C) Layer 3 – Network D) Layer 7 – Application 9\. Which protocol is used to securely manage and monitor network devices, replacing the insecure version 1/2c of its predecessor? A) SNMPv3 B) SNMPv1 C) Telnet D) RIP 10\. IPsec is most commonly used to provide secure communication at which OSI layer? A) Layer 3 – Network B) Layer 4 – Transport C) Layer 6 – Presentation D) Layer 7 – Application Answer Key B – Switches forward frames using MAC addresses, a Layer 2 function. C – DNS translates domain names to IP addresses. B – VPNs create encrypted tunnels over untrusted networks like the internet. B – The Session layer manages dialog control between applications. B – SSH provides encrypted remote access, replacing Telnet. B – TLS sits between Transport and Application, often described as operating at Layer 6/7 boundary in practice, though technically it's not a strict OSI layer. B – SFTP (SSH File Transfer Protocol) encrypts file transfers; FTP does not. A – The Physical layer handles the actual transmission of raw bits as signals. A – SNMPv3 added authentication and encryption, unlike v1/v2c. A – IPsec operates at the Network layer, securing IP packets. If you missed more than 2-3, your blind spot is likely protocol-to-layer mapping — that's the single highest-yield area to drill before the exam. Want me to generate a second, harder set focused specifically on that, or run through scenario-based questions instead?"

### **Notes**

| Category | Details |
| :---- | :---- |
| **What changed in the prompt** | Added specific user background context and established a clear motivation regarding Domain 4\. |
| **What improved in the output** | The output successfully narrowed its focus to deliver questions exclusively on Domain 4: Network Security, specifically targeting the OSI model and secure protocols. |
| **What still failed** | Claude still referenced the unrelated portfolio context in its introduction. The output did not natively structure the questions into complex, uniform scenarios. |
| **What to try next** | Introduce few-shot examples to dictate the exact style and complexity desired for the questions. |

## **Version 3 (+ Few-Shot Examples)**

### **Prompt**

`Act as an expert cybersecurity instructor who specializes in preparing students for the ISC2 Certified in Cybersecurity (CC) exam.`  
`I am an Information Systems student taking the ISC2 CC exam soon to transition into the cybersecurity field. I am struggling with Domain 4: Network Security, specifically concerning the OSI model and secure protocols. I need to test my knowledge to identify my blind spots so I don't fail the real exam.`  
`Here are some examples of the difficulty and style of questions I am looking for:`  
`Example 1:`  
`Q: At which layer of the OSI model does a router primarily operate?`  
`A) Data Link Layer`  
`B) Network Layer`  
`C) Transport Layer`  
`D) Application Layer`  
`Answer: B`  
`Example 2:`  
`Q: Which of the following protocols is considered inherently unsecure because it transmits data in plaintext?`  
`A) SSH`  
`B) HTTPS`  
`C) Telnet`  
`D) IPsec`  
`Answer: C`  
`Now, write 3 new practice questions for the ISC2 CC exam.`

### **Output Excerpt**

#### **Claude:**

"Happy to do both — let's knock out the cybersecurity questions first since that's self-contained, then dive into the portfolio interview. ISC2 CC Practice Questions — Domain 4: Network Security Q1: A network administrator needs to segment traffic between the Finance and HR departments to reduce the broadcast domain and improve security, without adding additional physical switches. Which technology should be used? A) VPN B) VLAN C) NAT D) DMZ Answer: B Q2: At which layer of the OSI model do switches primarily operate when making forwarding decisions based on MAC addresses? A) Physical Layer B) Data Link Layer C) Network Layer D) Session Layer Answer: B Q3: Which protocol should be used to securely transfer files over a network, replacing the plaintext FTP protocol? A) TFTP B) HTTP C) SFTP D) SNMP Answer: C A quick blind-spot check for you: the CC exam loves testing whether you know the replacement pair for insecure protocols (Telnet→SSH, FTP→SFTP/FTPS, HTTP→HTTPS, SNMPv1/v2→SNMPv3). If you can rattle those off cold, you're in good shape. Want me to keep drilling this domain (e.g., firewalls/IDS-IPS placement, or the specific layer functions like segmentation vs. encapsulation), or do you feel solid here now? Portfolio Case Study — Project Interview Let's build your first case study. I'll ask one question at a time, and I'll hold your Voice Card (direct, factual, blunt, no fluff) for the actual copy once we draft it. Question 1: Which project are we starting with, and in one sentence, what problem was it solving?"

### **Notes**

| Category | Details |
| :---- | :---- |
| **What changed in the prompt** | Added two examples displaying the precise formatting and style, and requested exactly 3 new questions. |
| **What improved in the output** | The output successfully adopted the instruction to output exactly 3 scenario-based questions. |
| **What still failed** | Claude continued to attach the unrelated portfolio case study interview to the end of its response. The visual output format was not strictly unified. |
| **What to try next** | Specify a strict output formatting template to enforce uniform visual structures and suppress unwanted conversational filler. |

## **Version 4 (+ Output Structure)**

### **Prompt**

`Act as an expert cybersecurity instructor who specializes in preparing students for the ISC2 Certified in Cybersecurity (CC) exam.`  
`I am an Information Systems student taking the ISC2 CC exam soon to transition into the cybersecurity field. I am struggling with Domain 4: Network Security, specifically concerning the OSI model and secure protocols. I need to test my knowledge to identify my blind spots so I don't fail the real exam.`  
`Here are some examples of the difficulty and style of questions I am looking for:`  
`Example 1:`  
`Q: At which layer of the OSI model does a router primarily operate?`  
`A) Data Link Layer`  
`B) Network Layer`  
`C) Transport Layer`  
`D) Application Layer`  
`Answer: B`  
`Example 2:`  
`Q: Which of the following protocols is considered inherently unsecure because it transmits data in plaintext?`  
`A) SSH`  
`B) HTTPS`  
`C) Telnet`  
`D) IPsec`  
`Answer: C`  
`Now, write 3 new practice questions for the ISC2 CC exam. Format your response exactly like this:`  
`Question [Number]: [Question text]`  
`A) [Option A]`  
`B) [Option B]`  
`C) [Option C]`  
`D) [Option D]`  
`Correct Answer: [Letter]`  
`Instructor's Explanation: [A brief 2-sentence explanation of why the answer is correct and why the distractors are wrong.]`

### **Output Excerpt**

#### **Claude:**

"Happy to help with both — let's knock out the exam prep first since it's self-contained, then I'll kick off the portfolio interview. ISC2 CC Practice Questions — Domain 4: Network Security Question 1: A network administrator wants to prevent unauthorized devices from communicating on the network by filtering traffic based on physical hardware addresses. At which OSI layer does this type of filtering primarily occur? A) Physical Layer B) Data Link Layer C) Network Layer D) Session Layer Correct Answer: B Instructor's Explanation: MAC address filtering happens at the Data Link Layer (Layer 2), since MAC addresses are Layer 2 identifiers used by switches. The Physical Layer only deals with raw bits and signaling, while the Network Layer (C) uses logical addressing (IP), not hardware addressing. Question 2: Which protocol should be used to securely transfer files over a network, replacing the plaintext FTP protocol? A) TFTP B) SFTP C) SNMP D) SMTP Correct Answer: B Instructor's Explanation: SFTP (SSH File Transfer Protocol) encrypts file transfers by running over SSH, directly addressing FTP's plaintext weakness. TFTP (A) is even less secure than FTP with no authentication, while SNMP (C) and SMTP (D) are unrelated to file transfer. Question 3: An organization wants to encrypt all IP traffic between two branch offices at the network layer, regardless of the application generating the traffic. Which protocol suite is best suited for this? A) SSL/TLS B) IPsec C) HTTPS D) SSH Correct Answer: B Instructor's Explanation: IPsec operates at the Network Layer and encrypts all IP packets between two endpoints, making it ideal for site-to-site VPNs regardless of the application in use. SSL/TLS (A) and HTTPS (C) operate higher in the stack and only secure specific application traffic, while SSH (D) is used for secure remote access to individual systems, not bulk network-to-network encryption. Portfolio Case Studies — Project 1 Interview Let's start with your first project. What was the project, and what problem were you actually trying to solve? (Not the tech stack yet — just: what was broken, missing, or needed, and for whom?)"

### **Notes**

| Category | Details |
| :---- | :---- |
| **What changed in the prompt** | Added a rigid output structure template dictating the placement of the questions, answer keys, and explanations. |
| **What improved in the output** | Claude utilized the correct headers ("Correct Answer:", "Instructor's Explanation:") as requested. |
| **What still failed** | Claude still ignored the implicit bounds of the formatting constraint by appending the portfolio case study interview to the very end of the output. |
| **What to try next** | Use step decomposition to guide the AI through a logical sequence, improving the distractors and completely finalizing the structure. |

## **Version 5 (+ Step Decomposition)**

### **Prompt**

`Act as an expert cybersecurity instructor who specializes in preparing students for the ISC2 Certified in Cybersecurity (CC) exam.`  
`I am an Information Systems student taking the ISC2 CC exam soon to transition into the cybersecurity field. I am struggling with Domain 4: Network Security, specifically concerning the OSI model and secure protocols. I need to test my knowledge to identify my blind spots so I don't fail the real exam.`  
`Here are some examples of the difficulty and style of questions I am looking for:`  
`Example 1:`  
`Q: At which layer of the OSI model does a router primarily operate?`  
`A) Data Link Layer`  
`B) Network Layer`  
`C) Transport Layer`  
`D) Application Layer`  
`Answer: B`  
`Example 2:`  
`Q: Which of the following protocols is considered inherently unsecure because it transmits data in plaintext?`  
`A) SSH`  
`B) HTTPS`  
`C) Telnet`  
`D) IPsec`  
`Answer: C`  
`Now, write 3 new practice questions for the ISC2 CC exam. To ensure high quality, follow these steps exactly:`  
`Step 1: Review the official objectives for ISC2 CC Domain 4 (Network Security).`  
`Step 2: Identify three distinct, highly testable concepts within this domain that were not covered in the examples.`  
`Step 3: Draft one scenario-based multiple-choice question for each of the three concepts. Ensure the distractors (incorrect options) are plausible but definitively incorrect.`  
`Step 4: Output the final questions using exactly the following format:`  
`Question [Number]: [Question text]`  
`A) [Option A]`  
`B) [Option B]`  
`C) [Option C]`  
`D) [Option D]`  
`Correct Answer: [Letter]`  
`Instructor's Explanation: [A brief 2-sentence explanation of why the answer is correct and why the distractors are wrong.]`

### **Output Excerpt**

#### **Claude:**

"Happy to help with both — let's knock out the ISC2 practice questions first, then start the portfolio interview. ISC2 CC Domain 4 — Practice Questions Step 1 (Domain review) / Step 2 (concepts not covered in your examples): Firewall architecture — stateful vs. stateless packet filtering VPN/tunneling — IPsec vs. SSL/TLS-based remote access Wireless security — WPA2/WPA3 vs. legacy WEP Step 3 & 4 (Questions): Question 1: A network administrator needs a firewall that can track the state of active connections and only allow return traffic that matches an established session. Which firewall type should they deploy? A) Packet-filtering firewall B) Stateful inspection firewall C) Proxy firewall operating only at Layer 7 D) Circuit-level gateway with no session tracking Correct Answer: B Instructor's Explanation: A stateful inspection firewall maintains a state table of active connections, so it can permit legitimate return traffic while blocking unsolicited packets. Packet-filtering firewalls (A) evaluate each packet in isolation with no memory of prior traffic, and D contradicts itself by describing a "circuit-level gateway" with no session tracking, which is not how that firewall type functions. Question 2: A company wants remote employees to securely access internal network resources as if they were physically on-site, with encryption applied at the network layer for all traffic. Which technology best fits this requirement? A) HTTPS B) IPsec VPN C) Telnet D) SNMP Correct Answer: B Instructor's Explanation: IPsec operates at the Network Layer (Layer 3\) and encrypts all IP traffic between endpoints, making it ideal for full network-level remote access. HTTPS (A) only secures individual web sessions rather than all network traffic, and Telnet (C) and SNMP (D) are not encryption/VPN technologies at all — Telnet is plaintext and standard SNMP lacks strong encryption. Question 3: A small office is upgrading its wireless network and wants the strongest available encryption and authentication standard to protect against offline dictionary attacks on the handshake. Which should they implement? A) WEP B) WPA C) WPA2-Personal D) WPA3-Personal Correct Answer: D Instructor's Explanation: WPA3 uses Simultaneous Authentication of Equals (SAE), which resists offline dictionary attacks against the handshake, a known weakness in WPA2's 4-way handshake. WEP (A) is broken and trivially crackable, and WPA (B) and WPA2 (C) are both weaker than WPA3, with WPA2 specifically vulnerable to the offline attack described in the question. Portfolio Case Study — Project 1 Let's start with your first project. What's the name of the project, and in one or two sentences, what problem were you trying to solve?”

#### **ChatGPT:**

"Question 1: A security administrator needs to ensure that DNS queries between clients and the DNS server cannot be easily intercepted or modified while in transit. Which protocol best addresses this requirement? A) DNS B) DNSSEC C) DoH (DNS over HTTPS) D) TFTP Correct Answer: C Instructor's Explanation: DoH encrypts DNS queries by sending them over HTTPS, protecting their confidentiality during transit. DNSSEC provides authentication and integrity for DNS records but does not encrypt queries, while DNS and TFTP transmit data without encryption. Question 2: A company wants to reduce the risk of unauthorized devices connecting to its wired network. Which technology is specifically designed to authenticate devices before granting network access? A) 802.1X B) NAT C) ARP D) SNMP Correct Answer: A Instructor's Explanation: IEEE 802.1X provides port-based Network Access Control (NAC), requiring authentication before a device is granted access to the network. NAT translates IP addresses, ARP resolves IP-to-MAC mappings, and SNMP is used for network monitoring and management rather than access control. Question 3: An attacker sends a large number of forged ARP replies to hosts on a local network, causing traffic to be redirected through the attacker's device. Which type of attack is being performed? A) DNS cache poisoning B) ARP spoofing C) SYN flooding D) Smurf attack Correct Answer: B Instructor's Explanation: ARP spoofing (or ARP poisoning) involves sending forged ARP messages to associate the attacker's MAC address with another host's IP address, enabling traffic interception. DNS cache poisoning targets DNS records, SYN flooding exhausts server connection resources, and a Smurf attack is an ICMP-based denial-of-service attack."

### **Notes**

| Category | Details |
| :---- | :---- |
| **What changed in the prompt** | Added step-by-step instructions to break the request down into logical phases. |
| **What improved in the output** | Claude explicitly displayed its reasoning for Steps 1 and 2 before outputting the questions. The generated questions featured high-quality distractors and detailed explanations based on the requested steps. |
| **What still failed** | Claude retained the unrelated portfolio case study text at the conclusion of its output. |
| **What to try next** | Distill this prompt into a final, context-free template. |

## **Cross-Model Comparison (Claude vs. ChatGPT)**

| Aspect | Claude | ChatGPT |
| :---- | :---- | :---- |
| **Tone** | Conversational and accommodating. It retains a chatty persona ("Happy to help with both — let's knock out the ISC2 practice questions first..."). | Strictly professional, direct, and clinical. It offers zero conversational filler or introductory pleasantries. |
| **Accuracy** | High. The questions covering stateful firewalls, IPsec, and WPA3 are highly relevant to Domain 4\. The distractors are plausible, and the explanations are factually sound. | High. The questions covering DoH, 802.1X, and ARP spoofing are excellent, highly testable concepts. The explanations clearly justify the correct choices. |
| **Structure** | **Format Violation:** Explicitly printed its reasoning for Step 1 and Step 2 before drafting the questions. By doing this, it technically violated the strict output template constraint requested in Step 4\. | **Perfect Compliance:** Executed Steps 1, 2, and 3 internally and output only the final result. It followed the strict formatting constraint of Step 4 perfectly without printing unrequested background steps. |
| **Failure Points** | **Context Bleed & Over-generation:** Failed to constrain its output. It appended the completely unrelated "Portfolio Case Study" task to the end of the response, proving it struggles to drop prior contextual baggage. It also over-generated by printing its internal reasoning steps instead of sticking exclusively to the requested template. | **None (Flawless Execution):** ChatGPT followed all instructions perfectly for Version 5\. It executed the background steps internally and output exactly the format requested in Step 4 without any context bleed, conversational filler, or structural errors. |

## **Final Reusable Prompt**

`Act as an expert instructor for the [Certification/Exam Name].`  
`I am a [User Background/Level] studying for this exam to achieve [Goal/Motivation]. I am currently struggling with [Specific Subject/Domain] and need to test my knowledge.`

`Here are examples of the difficulty and style I need:`  
`Example 1: [Insert Example Q&A]`  
`Example 2: [Insert Example Q&A]`

`Write [Number] new practice questions. Follow these steps exactly:`  
`Step 1: Review the core objectives for [Specific Subject/Domain].`  
`Step 2: Identify [Number] highly testable concepts.`  
`Step 3: Draft a multiple-choice question for each concept, ensuring distractors are plausible but incorrect.`  
`Step 4: Output the final questions using this exact format:`

`Question [Number]: [Question text]`  
`A) [Option A]`  
`B) [Option B]`  
`C) [Option C]`  
`D) [Option D]`

`Correct Answer: [Letter]`  
`Instructor’s Explanation: [2-sentence explanation of correct vs. incorrect options]`