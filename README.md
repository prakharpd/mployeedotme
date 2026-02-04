# Resume Bullet Rewriter Using LLM 

This system processes user-provided resume bullet points and transforms them using multiple Large Language Models (LLMs) via OpenAI-compatible APIs, with an emphasis on evaluating model performance and prompt effectiveness.

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

**gpt-oss:120b-cloud**

It produced the most consistent, professional, and well-structured outputs with minimal hallucination.

---

## Prompting Strategies

Four strategies were tested:

1. Zero-shot  
2. Few-shot  
3. Chain-of-thought  
4. Role-based (resume consultant)

Few-Shot, Chain-of-Thought and Role-based prompting gave the best overall results.

---

## Challenges Faced

- Metric hallucination (fake percentages).  
- Over-instruction reducing output quality.  
- Evaluation bias when varying model and prompt together.  
- Exact model tags required in Ollama (no fallback handling).

---

## Conclusion

Prompt design and LLM model used had more impact on the result. 
Higher the parameter used for training the LLM better would be the result.
Local models, especially **gpt-oss:120b-cloud**, can be used for real resume rewriting tasks.
Since they are fast and computationally efficient.
