# 🛡️ Guardrails AI Demonstration

This repository contains a comprehensive Jupyter Notebook demonstrating how to use **Guardrails AI** to add safety, reliability, and structural guarantees to Large Language Model (LLM) outputs. The notebook showcases how Guardrails can be used to validate responses, enforce schemas, detect unsafe or sensitive content, and integrate with external tools such as Microsoft Presidio and spaCy.

This project is part of my personal GitHub portfolio and highlights my practical understanding of **LLM safety, validation pipelines, and production-ready AI systems**.

---

## 📌 What is Guardrails AI?

**Guardrails AI** is an open-source framework designed to:

* Enforce **structured outputs** from LLMs
* Validate content using **schemas** (JSON, Pydantic, etc.)
* Add **safety checks** (profanity, PII, toxicity, etc.)
* Automatically **re-ask** the LLM when constraints are violated
* Integrate with popular LLM providers and local models

It is commonly used in:

* Chatbots
* RAG systems
* AI agents
* Form-filling workflows
* Enterprise LLM pipelines

---

## 🎯 Objectives of This Notebook

This notebook demonstrates how to:

1. Enforce **structured outputs** using Guardrails schemas
2. Validate model responses for **consistency and correctness**
3. Detect and block **profanity or unsafe language**
4. Identify and protect **PII (Personally Identifiable Information)**
5. Integrate **Microsoft Presidio** for privacy detection
6. Use **spaCy NLP models** for linguistic processing
7. Run Guardrails with **local or remote LLMs** via LiteLLM

---

## 🧠 Key Concepts Demonstrated

### 1. Schema Validation

LLMs typically return unstructured text. Guardrails enforces strict schemas so outputs become:

* Machine-readable
* Predictable
* Programmatically safe

This is essential for production systems.

---

### 2. Content Moderation

The notebook demonstrates how Guardrails can prevent:

* Profanity
* Hate speech
* Abusive or unsafe content

This ensures that generated responses remain safe, ethical, and user-friendly.

---

### 3. PII Detection with Microsoft Presidio

Microsoft Presidio is used to detect sensitive information such as:

* Phone numbers
* Email addresses
* Credit card numbers
* Names
* Locations

This is critical for privacy-preserving AI systems.

---

### 4. NLP Processing with spaCy

spaCy’s large English model (`en_core_web_lg`) is used for:

* Tokenization
* Lemmatization
* Named Entity Recognition (NER)
* Linguistic analysis

---

### 5. Local & Remote Model Support

This notebook supports both:

* Cloud-based LLMs (OpenAI, etc.)
* Local models (Ollama, llama.cpp, Hugging Face)

Using **LiteLLM**, you can easily switch between providers.

---

## 🛠️ Technologies Used

| Tool / Library     | Purpose                     |
| ------------------ | --------------------------- |
| Guardrails AI      | Output validation & safety  |
| LiteLLM            | Unified LLM interface       |
| Microsoft Presidio | PII detection               |
| spaCy              | NLP processing              |
| Jupyter Notebook   | Interactive experimentation |
| Python             | Core language               |

---

## 🚀 How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2. Install Dependencies

```bash
pip install guardrails-ai litellm presidio-analyzer presidio-anonymizer spacy
python -m spacy download en_core_web_lg
```

### 3. Configure Guardrails (Optional)

```bash
guardrails configure
```

### 4. Launch Notebook

```bash
jupyter notebook
```

---

## 📓 Notebook Contents

The notebook walks through:

1. Introduction to Guardrails
2. Schema-based output validation
3. Profanity filtering
4. PII detection
5. Integration with NLP tools
6. Local model usage
7. Error handling & re-asking
8. Best practices

---

## 🧪 Example Use Case

Instead of this:

> "Here is some random unstructured text"

You get this:

```json
{
  "name": "John Doe",
  "age": 32,
  "email": "[REDACTED]"
}
```

With automatic validation and correction.

---

## 🔐 Why Guardrails Matters

In production AI systems, **hallucinations and unsafe outputs are unacceptable**.

Guardrails helps by:

* Preventing invalid responses
* Enforcing formats
* Improving reliability
* Enhancing user trust
* Reducing compliance risk

---

## 🌟 Portfolio Value

This project demonstrates:

* Applied AI safety engineering
* Real-world LLM reliability practices
* Data privacy awareness
* Modern NLP tooling
* Production-style AI workflows

---



---

⭐ If you found this useful, please star the repo!
