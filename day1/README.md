"# Agentic-Ai" 
# Day 1 – How LLMs Work and Your First API Call

## 📌 About This Project

This project is part of the **AI Agents Workshop – Level 1 Fundamentals**.

The goal is to understand how Large Language Models (LLMs) work, learn the fundamentals of AI engineering, and make our first API call using Python.

This beginner-friendly tutorial covers essential AI concepts through real-world examples, interactive demonstrations, animations, and quizzes.

## 🎯 Learning Objectives

By completing this tutorial, you will learn:

- How modern AI applications work.
- What Large Language Models (LLMs) are.
- How LLMs generate responses using next-token prediction.
- What tokens are and how they affect API costs.
- What temperature means and how it controls response creativity.
- Why LLMs do not automatically remember previous API calls.
- What a context window is.
- What hallucinations are and how to reduce them.
- What an AI engineer does.
- How to make your first LLM API call using Python.

## 📚 Topics Covered

| No. | Topic | Description |
|---|---|---|
| 01 | Why AI is Everywhere | Understanding the growth of AI and APIs |
| 02 | What is an LLM? | Understanding next-token prediction |
| 03 | Tokens | How text is divided into smaller pieces |
| 04 | Temperature | Controlling creativity and randomness |
| 05 | No Memory | Understanding conversation history |
| 06 | Context Window | Understanding token limits |
| 07 | Hallucination | Why AI generates incorrect information |
| 08 | AI Engineer | Understanding the role of an AI engineer |
| 09 | First API Call | Connecting to an LLM using Python |

## 🛠️ Technologies Used

- **Python** – Programming language.
- **Google Colab** – Cloud-based Python environment.
- **LLM API** – Accessing a pre-trained language model.
- **HTML, CSS and JavaScript** – Interactive learning experience.

## 🧪 Practical Learning

The tutorial uses a fictional business called **Sweet Crumbs Home Bakery** as a case study.

The bakery receives cake orders through chat and repeatedly answers customer questions.

The objective is to understand how AI can help automate its operations through:
- Marketing Agent
- Sales & Support Agent
- Operations Agent

Day 1 focuses on building the foundation by making an API call that answers bakery-related questions.

## 💻 First API Call

The tutorial demonstrates how to connect to an LLM using Python.

Example:

```python
response = client.chat.completions.create(
    model="openai/gpt-oss-20b",
    temperature=0.2,
    messages=[
        {"role": "system", "content": SYSTEM},
        {
            "role": "user",
            "content": "Can I get an eggless cake today evening?"
        }
    ],
)

print(response.choices[0].message.content)
print(response.usage)
```

This demonstrates how to:
1. Select an AI model.
2. Set the temperature.
3. Provide system instructions.
4. Send a user message.
5. Receive the model's response.
6. Check token usage.

## 🚀 How to Get Started

1. Open the tutorial HTML file in your browser.
2. Follow the nine topics in order.
3. Explore the interactive demonstrations and animations.
4. Complete the quizzes after each topic.
5. Open Google Colab for the Python API exercise.
6. Experiment with different prompts and temperature values.

## 📝 Hands-on Exercises

- Compare responses at temperature 0.2 and 1.2.
- Observe hallucinations by removing factual information from the prompt.
- Test how conversation history affects memory.
- Compare token usage between English and Telugu.
- Create a system prompt for your own business.

## 📖 Key Takeaways

By the end of Day 1, you should understand:

- An LLM predicts the next token repeatedly to generate text.
- Tokens are the basic units used for processing and generating text.
- Temperature controls the randomness of generation.
- Conversation history must be supplied again when needed.
- Context windows limit how much information a model can process in one request.
- AI engineers build applications using existing models rather than necessarily training their own models.
- APIs allow developers to integrate AI capabilities into applications.

## 🔮 What's Next?

**Day 2 – Building AI Agents**

The next session builds on these fundamentals to create an AI-powered application using system prompts, conversation memory, and testing.

---

**Learning Track:** AI Agents Workshop  
**Level:** Beginner – Level 1 Fundamentals  
**Day:** 1 of 2  
**Duration:** Approximately 2 hours

*Learn the fundamentals. Experiment with prompts. Build with AI.*