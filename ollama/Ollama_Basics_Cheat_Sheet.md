# 🧠 Ollama Basics Cheat Sheet

This guide covers the essential commands for getting started with [Ollama](https://ollama.com), a tool that lets you run large language models locally on your machine.

---

## 📦 1. Pull a Model

```bash
ollama pull llama3
```

Downloads the model (e.g., `llama3`) to your machine so you can use it locally. Other model names include `mistral`, `gemma`, and `phi`.

---

## 💬 2. Run a Chat with a Model

```bash
ollama run llama3
```

Starts a terminal-based chat with the model you downloaded. You can interact with it like you would in ChatGPT, but it's fully local.

---

## 📄 3. Create a Custom Model

```bash
ollama create mymodel -f Modelfile
```

Builds a new model variant using a `Modelfile`. This lets you customize the system prompt or settings.

**Example Modelfile:**
```
FROM llama3
SYSTEM "You are a helpful math tutor."
```

---

## 📋 4. List Installed Models

```bash
ollama list
```

Displays all the models you've downloaded and made available locally.

---

## 🧹 5. Remove a Model

```bash
ollama remove llama3
```

Deletes a model from your system to save disk space.

---

## 🔄 6. Update Ollama

```bash
ollama update
```

Updates the **Ollama tool itself** (not the models) to the latest version. Useful for getting new features and bug fixes.

---

## 🌐 7. Serve as an API (Advanced)

```bash
ollama serve
```

Starts an API server that lets other apps or code interact with your local models via HTTP. This is useful for developers.

---

## ✅ Tips

- **Exit a chat:** Press `Ctrl+C`
- **Help menu:** `ollama help`
- Ollama runs models **entirely locally** — no internet required after pulling a model.
- Models can be several GB, so make sure you have space.

---

## 🚀 Start Here

1. Install from [https://ollama.com/download](https://ollama.com/download)
2. Run in terminal:
    ```bash
    ollama pull llama3
    ollama run llama3
    ```
3. You’re chatting with an LLM locally!

---
