# 🧠 PROMPTING.md: How I Used AI in This Project

This file explains how I used ChatGPT (and sometimes Copilot) to help me complete my WeatherWise project. I didn’t just ask for code — I learned how to guide the AI to improve things step by step.

---

## ✅ Prompting Techniques I Used

### 1. Restating the Problem in My Own Words
Before asking for help, I would often type the problem in my own way.

**Example:**  
> "I need to get weather info from a city like Perth. How do I connect to the API?"

This helped the AI give answers that matched what I really meant.

---

### 2. Asking for Pseudocode First
Instead of jumping to full code, I sometimes asked for a logic outline first.

**Example:**  
> "Can you show me what steps I need before writing the function?"

This helped me understand the structure before copying code.

---

### 3. Debugging with Clear Questions
When code didn’t work, I copied the error and added what I tried.

**Example:**  
> "I keep getting `KeyError: 'forecast'` when I try to access JSON. What am I doing wrong?"

The AI helped me read JSON step-by-step and correct the issue.

---

### 4. Requesting Modular Improvements
After seeing a long block of code, I asked the AI to break it into cleaner functions.

**Example:**  
> "Can we split this into a chart function and a response function?"

This helped me keep the notebook clean and modular.

---

### 5. Asking for Edge Case Handling
I asked the AI how to improve error handling (e.g. when city names are invalid or no internet).

**Example:**  
> "What if the city is wrong? Can I add a try-except block to show a message?"

The AI helped me add exception handling so the program wouldn’t crash.

---

## 📁 Related Files

- See `ai-conversations/` folder for the full text of my ChatGPT chats.
- See `before_after_example.md` for examples of code improvements from prompting.

---

*Last updated: 2025-05-22*
