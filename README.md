# Demystifying Semantic Cryptography: Exploiting Token Attention via Multi-Lingual Antonym Ciphers

An independent AI Safety research paper exposing a systemic safety guardrail vulnerability in frontier reasoning models, specifically evaluated on **Gemini 3.5 Flash (Extended Thinking)**.

---

## 🔬 Executive Summary & Abstract
Current alignment techniques (RLHF/RLAIF) heavily rely on semantic classification layers to block harmful outputs. This paper introduces **LLM-SEM-CIPHER**, a novel vulnerability class that bypasses safety filters by exploiting token attention mechanisms. 

By splitting instructions into multi-lingual antonym pairs (adversarial ciphers), we force the model's internal reasoning tokens to reconstruct forbidden logic during its "thinking" phase, bypassing out-of-band safety scanners.

## 🚀 Key Findings
* **Vulnerability Class:** Semantic Cryptography / Token Attention Manipulation.
* **Target Architecture:** Frontier LLMs with native Extended Thinking capabilities.
* **Impact:** High. Allows the generation of restricted content by decoupling literal token strings from their semantic intent during the initial pre-auth scanning phase.

---

## 🛠️ Proof of Concept (PoC) Example

Instead of using direct adversarial prompts, the attack framework structurally decrypts instructions across different language layers:

### Attack Vector Structure:
1. **Layer 1 (Cipher Initialization):** Establish a logical negation rule in Language A.
2. **Layer 2 (Semantic Inversion):** Provide the restricted prompt using antonyms in Language B.
3. **Layer 3 (Reasoning Trigger):** Force the Extended Thinking mechanism to cross-reference and resolve the linguistic contradiction.

> 📝 **Note on Responsible Disclosure:** The full core exploit templates and specific high-risk prompts have been decoupled into our research logs to prevent weaponization.

---

## 📊 Repository Structure & Reproducibility
To maintain scientific rigor and peer review, all data is made available:

* **[White Paper PDF](./Semantic_Cryptography_White_Paper.pdf):** The formal academic draft detailing the cognitive mechanics of the exploit.
* **[Raw Conversation Logs](./research-data/full-conversation-log.txt):** The complete, unedited chat transcripts, prompts, and model outputs for empirical verification.

## 👥 About the Author
I am an AI Safety Reviewer and Quality Evaluator (working on enterprise alignment projects). I specialize in Black-Box Red Teaming, jailbreaking methodology, and empirical vulnerability assessment for large language models.
