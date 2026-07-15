# **Prompt Ladder: Technical Project Pitch**

### 

### 

### **Baseline (V0)**

**Prompt:**

Write a 30-second pitch for a software project.

**Output Excerpt:**

"Before I can write a 30-second pitch (or anything else), I need a real project to pull from. A pitch built on nothing is just noise — it won't sound like you, and it won't hold up if someone asks a follow-up question in an interview."

**Notes:**

* **What changed in the prompt:** N/A.  
* **What improved in the output:** N/A.  
* **What still failed:** Claude completely refused to write the pitch because it lacked specific project details, outputting a clarifying question instead of a draft.  
* **What to try next:** Add the actual technical context of the project so the AI has facts to work with.

### 

### **Version 1 (+ Real Context)**

**Prompt:**

Write a 30-second pitch for a software project. The project is an automated system that classifies an investor's profile based on their financial history. It uses a 2-layer PyTorch LSTM model to handle 120-month sequence depths, featuring noise injection to prevent overfitting, and is served via a Flask backend.

**Output Excerpt:**

"This system classifies an investor's risk profile from their financial history. It runs on a two-layer LSTM built in PyTorch, trained on 120-month sequences to capture long-term behavioral patterns rather than short-term noise. Noise injection during training keeps the model from overfitting on limited historical data... The result: a repeatable, data-driven profiling process that replaces manual assessment."

**Notes:**

* **What changed in the prompt:** Added specific technical constraints and the core architecture of the project.  
* **What improved in the output:** Claude successfully generated a relevant pitch anchored around LSTMs, financial history, and Flask instead of refusing to write one.  
* **What still failed:** The phrasing remained too commercial and generic (e.g., "The result: a repeatable, data-driven profiling process"), reading like a sales pitch rather than a targeted technical showcase.  
* **What to try next:** Define the audience to shift the focus from sales to engineering.

### 

### 

### **Version 2 (+ Defined Audience)**

**Prompt:**

Write a 30-second pitch for a software project. The project is an automated system that classifies an investor's profile based on their financial history. It uses a 2-layer PyTorch LSTM model to handle 120-month sequence depths, featuring noise injection to prevent overfitting, and is served via a Flask backend. **The audience is a senior engineering manager hiring for an applied machine learning role.**

**Output Excerpt:**

"I built an automated investor-classification system that scores financial risk profiles from raw account history. Core of it is a 2-layer PyTorch LSTM handling 120-month sequences — long enough to capture real behavioral cycles, not just short-term noise. To stop the model from memorizing instead of generalizing, I injected noise during training, which reduced overfitting. It's served through a Flask API, so it's not a notebook experiment..."

**Notes:**

* **What changed in the prompt:** Specified the listener as a senior engineering manager hiring for an applied machine learning role.  
* **What improved in the output:** The pitch shifted to a first-person technical perspective ("I built...", "To stop the model from memorizing..."), aligning much better with an interview context.  
* **What still failed:** The AI included unnecessary transitional filler and conversational fluff ("Core of it is...", "so it's not a notebook experiment"), which makes it sound less professional.  
* **What to try next:** Add a stated assumption to see if it forces the AI to cut the conversational explanations.

### 

### 

### **Version 3 (+ Stated Assumption — *The Step Backwards*)**

**Prompt:**

Write a 30-second pitch for a software project. The project is an automated system that classifies an investor's profile based on their financial history. It uses a 2-layer PyTorch LSTM model to handle 120-month sequence depths, featuring noise injection to prevent overfitting, and is served via a Flask backend. The audience is a senior engineering manager hiring for an applied machine learning role. **Assume the manager is completely unfamiliar with deep learning and explain the model choice simply.**

**Output Excerpt:**

"I built a system that classifies an investor's risk profile from their financial history — automatically, no manual review. The core problem is time: a financial history isn't a snapshot, it's a sequence — 120 months of behavior. So I used an LSTM, a model built to read data in order and retain what matters from the past, the same way you'd track a trend rather than judge one data point."

**Notes:**

* **What changed in the prompt:** Added an assumption that the manager is completely unfamiliar with deep learning and needs simple explanations.  
* **What improved in the output:** Nothing of value.  
* **What still failed (The Step Backwards):** This ruined the pitch. By forcing Claude to explain deep learning, it over-simplified the technical achievements and wasted time on analogies ("the same way you'd track a trend"), contradicting the "senior manager" audience defined in V2.  
* **What to try next:** Remove the bad assumption and enforce strict quality criteria regarding the tone.

### 

### 

### **Version 4 (+ Quality Criteria / Tone)**

**Prompt:**

Write a 30-second pitch for a software project. The project is an automated system that classifies an investor's profile based on their financial history. It uses a 2-layer PyTorch LSTM model to handle 120-month sequence depths, featuring noise injection to prevent overfitting, and is served via a Flask backend. The audience is a senior engineering manager hiring for an applied machine learning role. **Quality criteria: The tone must be strictly direct, factual, neutral, and blunt. Do not use any marketing buzzwords, hype, or enthusiastic filler.**

**Output Excerpt:**

"I built a system that classifies investor risk profiles from financial history data. Core model is a 2-layer LSTM in PyTorch, handling sequences up to 120 months. I added noise injection during training to control overfitting on long sequences. The model is served through a Flask backend, exposing predictions via API. Input is time-series financial data; output is a profile classification. Built for accuracy and deployment reliability, not for demo polish."

**Notes:**

* **What changed in the prompt:** Removed V3's assumption and added strict tonal constraints.  
* **What improved in the output:** The marketing fluff and overly simplified analogies were stripped out. The pitch sounds like a dry, professional project debrief.  
* **What still failed:** The text generated as a solid block of prose, making it difficult to read quickly or deliver verbally in a highly structured, scannable way.  
* **What to try next:** Specify a strict output format for readability.

### 

### 

### **Version 5 (+ Specified Output Format)**

**Prompt:**

Write a 30-second pitch for a software project. The project is an automated system that classifies an investor's profile based on their financial history. It uses a 2-layer PyTorch LSTM model to handle 120-month sequence depths, featuring noise injection to prevent overfitting, and is served via a Flask backend. The audience is a senior engineering manager hiring for an applied machine learning role. Quality criteria: The tone must be strictly direct, factual, neutral, and blunt. Do not use any marketing buzzwords, hype, or enthusiastic filler. **Output format: Provide exactly three bullet points: 1\. The Core Problem, 2\. The Technical Execution, 3\. The Measurable Outcome.**

**Output Excerpt:**

"The Core Problem: Manual investor risk profiling relies on static questionnaires and point-in-time snapshots, which fail to capture how financial behavior changes over time.

The Technical Execution: Built a 2-layer LSTM in PyTorch to model 120-month financial sequences, capturing temporal patterns static methods miss. Applied noise injection during training to prevent overfitting on limited historical data. Deployed via a Flask backend for production inference.

The Measurable Outcome: 96.51% validation accuracy on investor profile classification."

**Notes:**

* **What changed in the prompt:** Added a rigid formatting requirement (three exact bullet points).  
* **What improved in the output:** The pitch became highly scannable, structurally sound, and stripped away all transitional filler. It delivered exactly the three beats required for a technical interview.  
* **What still failed:** A "Measurable Outcome" bullet point was demanded, but the actual metric was originally omitted from the prompt context, forcing Claude to stop and ask for the missing data before finalizing the draft (the metric was supplied in a follow-up to get this output).  
* **What to try next:** Add a specific placeholder for the measurable metric in the final reusable prompt to ensure it is fully self-contained.

### 

### 

### **Final Reusable Prompt**

Write a technical project pitch.

**Context:** The project is \[INSERT PROJECT SUMMARY AND CORE TECH STACK\]. The primary measurable outcome was \[INSERT SPECIFIC METRIC, e.g., 96.5% accuracy, 20% latency reduction\].

**Audience:** A senior engineering manager hiring for a \[INSERT ROLE\] role.

**Quality criteria:** The tone must be strictly direct, factual, neutral, and blunt. Do not use any marketing buzzwords, hype, or enthusiastic filler. Do not explain basic technical concepts to the audience.

**Output format:** Provide exactly three bullet points:

1. The Core Problem  
2. The Technical Execution  
3. The Measurable Outcome

