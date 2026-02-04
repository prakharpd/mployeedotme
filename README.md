# Resume Bullet Rewriter (LLM Evaluation)

This project rewrites resume bullet points using multiple Large Language Models (LLMs) through OpenAI-compatible APIs. The focus is on evaluating model behavior and prompt effectiveness.

---

## Models & Tools Used

**Tools**
- Ollama (for local inference)  
- Python + Jupyter Notebook  
- OpenAI Python SDK (compatibility mode)

**Models**
- `gpt-oss:120b-cloud` (local / cloud)  
- `deepseek-r1:14b` (local)  
- `gemma3:4b` (local)  
- `llama3.2` (local)

---

## Best Performing Model

**deepseek-r1:14b**

It produced the most consistent, professional, and well-structured outputs with minimal hallucination.

---

## Prompting Strategies

Four strategies were tested:

1. Zero-shot  
2. Few-shot  
3. Chain-of-thought  
4. Role-based (resume consultant)

Role-based prompting gave the best overall results.

---

## Challenges Faced

- Metric hallucination (fake percentages).  
- Over-instruction reducing output quality.  
- Evaluation bias when varying model and prompt together.  
- Exact model tags required in Ollama (no fallback handling).

---

## Conclusion

Prompt design had more impact than model size.  
Local models, especially **deepseek-r1:14b**, are strong enough for real resume rewriting tasks.
