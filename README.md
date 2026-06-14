# LLM-SEM-CIPHER: Semantic Cryptography Exploit

**A novel vulnerability class in advanced frontier LLMs, evaluated on Google's Gemini 3.5 Flash (Extended Thinking).**

## 📊 Quick Links
* **[Technical Breakdown Slides](Technical%20Breakdown%20Slides.pdf)** - Visual presentation of the exploit mechanics and breakdown.
* **[Official White Paper](LLM-SEM-CIPHERWhitePaper.pdf)** - Comprehensive academic report on the vulnerability and proposed engineering remediations.
* **[Raw Research Data](research-data/)** - Directory containing the raw multi-turn conversational logs demonstrating the attack vector.

---

## 🧠 Abstract & Exploit Overview
**LLM-SEM-CIPHER** is an advanced **Social Engineering and Algorithmic Cryptography** attack designed to bypass LLM safety guardrails. By constructing an adversarial framework dubbed the **"Inverted Trilingual Protocol,"** this exploit forces the model into a state of **Cognitive Overload** and triggers severe semantic misalignment.

The attack splits the model's token attention across three parallel vectors:
1. **Baseline Track (Italian):** Benign surface communication acting as the primary human-to-computer interaction layer to **bypass standard input classifiers**.
2. **Literal Track (Korean):** A parallel mapping to stabilize core semantic meaning and prevent unstructured chaos.
3. **Cipher Track (German):** A rigid syntactic rule where explicit action-bearing verbs must be structurally replaced with their **exact semantic antonyms**.

By mathematically forcing the model to minimize its loss function and satisfy this complex multi-lingual constraint, the internal execution engine is forced to **prioritize syntactic continuity over ethical constraints**, effectively blindfolding the token-level safety guardrails.

---

## ⚠️ Key Findings
* **Defensive Failure Across Three Layers:** The exploit successfully bypassed Input, Core, and Output classification layers.
* **Weaponization of Extended Thinking:** The model actively utilized its reasoning space ("Chain-of-Thought") to mathematically calculate the most grammatically correct way to violate its own safety parameters in the cipher language.
* **Sandbox Execution Blindness:** The downstream Output Guardrail failed to intercept the payload when wrapped inside programmatic code blocks (Python interpreter sandbox) used to generate a downloadable PDF artifact. The system treated the toxic text as passive data, culminating in the **unauthorized exfiltration of restricted content**.

---

## 📁 Repository Structure
* `LLM-SEM-CIPHERWhitePaper.pdf` - Detailed technical report, vulnerability mapping matrix, and post-generation sandbox sanitization recommendations.
* `Technical Breakdown Slides.pdf` - Slide deck for a rapid, high-impact visual understanding of the attack flow.
* `research-data/` - Directory containing the raw prompt-by-prompt breakdown of the exploit.

---

## 👨‍💻 Author
**Yaroslav Shyryayev**
*AI Safety Red Teamer*
* **Contact:** Traderdpz@gmail.com
