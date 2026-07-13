# Portfolio Sitemap + Toolkit: Setup and Audit

## 1. Portfolio Sitemap Design
Below is the digital sitemap structured for a minimalist, single-page scrolling portfolio.

![Portfolio Sitemap](Portfolio_Sitemap.png)<img width="962" height="824" alt="Portfolio_Sitemap" src="https://github.com/user-attachments/assets/c92fc500-de2a-4043-bca1-10d18472f887" />

* **Hero / Landing**: States the core claim and immediate call to action.
* **Projects / Work**: Displays technical proof-of-work (Buffet Brain, Jarvis, Transcriptor).
* **About**: Validates academic background and path.
* **Contact**: Houses the single desired action.

---

## 2. Claude Project Configuration
Here is the configured Claude Project workspace and custom instructions used for ongoing tutoring and evaluation.

### Project Workspace View
![Claude Project Portfolio](Claude_project_portfolio.png)<img width="1918" height="958" alt="Claude_project_portfolio" src="https://github.com/user-attachments/assets/98682a77-515a-4211-9d7f-a95178abbd09" />

### Custom Instructions Set
![Instruções Projeto Portfolio](Instruções_projeto_portfolio.png)<img width="736" height="524" alt="Instruções_projeto_portfolio" src="https://github.com/user-attachments/assets/8e50954a-eaa1-4b9a-8d27-d368dcf16cd8" />




> **Custom Instructions Used:**
> *Act as a Tutor for an IT student who needs your help to build a SPA (single page application) that showcases his portfolio, you will analyze the sitemaps shown to you and give an honest, unbiased review, by listing negative and positive observations and features, you will then offer solutions to any issues that are found, by recommending changes to the structure of the sitemap. Also you will need to pressure-test the sitemap and the portfolio of the student by comparing the claims made and actions that affirm them.*

---

## 3. Pressure-Test Prompt and Output

### The Prompt
> **My Core Claim:** I am an Information Systems student building practical expertise in AI engineering and foundational cybersecurity, focusing on delivering intelligent systems and robust technical solutions.
>
> **The One Desired Action:** I want a recruiter, tech lead, or peer to click my "Contact" or "Get in Touch" button to reach out for an internship or project collaboration.
>
> **My Sitemap Structure (from top to bottom):**
> * **Hero Section:** States my core claim and introduces who I am with an immediate call to action to view work.
> * **Projects / Work:** Displays high-impact technical proof—highlighting AI/ML work like Buffet Brain, the voice assistant Jarvis, and the Transcriptor project, alongside an introductory cybersecurity or secure-coding lab/module—to back up the dual claim.
> * **Skills:** A scannable stack overview showcasing both AI and basic security tools side by side.
> * **About:** Validates my active academic path, foundational learning, and technical foundation.
> * **Contact:** Houses the single desired action with direct links and a resume download.
>
> **Pressure-Test Prompt:** Please critique this updated sitemap flow and aligned claim against my single desired action. Does balancing the cybersecurity scope with foundational evidence and adding a skills strip successfully resolve the credibility gap while keeping the focus tight on driving that final contact action?

### Claude's Output
Good sitemap to work with — it's already thinking in terms of "claim $\rightarrow$ evidence $\rightarrow$ action," which most student portfolios don't do. Let me pressure-test it properly rather than just validate it.

#### What's Working
1. **Hero $\rightarrow$ Projects $\rightarrow$ Contact skeleton is sound.** You've correctly identified that recruiters skim, so proof-of-work needs to sit right after the intro.
2. **Pairing skills with projects, not replacing them.** Backing a skills strip with named projects (Buffet Brain, Jarvis, Transcriptor) is the right instinct.
3. **Single CTA discipline.** One desired action (Contact), resume download bundled into it rather than floating separately.

#### Where It Breaks Down
1. **Your core claim has two legs, and one leg is much shorter than the other.** Three AI/ML projects and one singular intro lab do not make a balanced dual claim.
2. **"Skills" as a standalone section after Projects is redundant unless it does new work.** If it just re-lists tools without context, let Projects carry the stack-proof.
3. **About is doing the wrong job in the wrong place.** It reads as biography filler unless it explains *why* the dual claim makes sense as one coherent person.
4. **One CTA button does not equal one CTA moment.** Relying 100% on scroll completion hurts conversion odds. Add a sticky nav or repeated soft CTA.

#### Direct Answer to Your Pressure-Test Question
No — reordering and adding a skills strip resolves the navigation problem, but it does not resolve the evidentiary credibility gap. You cannot structure your way out of a lopsided evidence-to-claim ratio.
