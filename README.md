# My HuggingFace Chatbot

A simple chatbot built with **[Hugging Face Transformers](https://github.com/huggingface/transformers)** and **[Gradio](https://github.com/gradio-app/gradio)**

---

## Table of Contents

1. [Overview](#overview)  
2. [Tech Stack](#tech-stack)  
3. [Installation](#installation)  

---

## Overview

This project uses the **Zephyr-7B** model via the `HuggingFaceH4/zephyr-7b-beta` Inference API. By leveraging the **InferenceClient** from `huggingface_hub`, we can stream the model’s tokens in real-time and display them in a **Gradio** chat interface. The chatbot includes adjustable parameters like **max tokens**, **temperature**, and **top-p** to control the generation process. Additionally, it supports a **system message**, which you can customize to guide the chatbot’s personality or style.

**Key Goals**:
- Demonstrate how to integrate the Zephyr-7B model using the `huggingface_hub` Inference API.
- Showcase streaming text responses in a user-friendly Gradio chat interface.
- Allow customization of generation parameters (max tokens, temperature, top-p) directly in the UI.


---

## Tech Stack

1. **Python 3**  
   The primary programming language.

2. **[huggingface_hub](https://github.com/huggingface/huggingface_hub)**  
   - Provides the `InferenceClient` for accessing and streaming responses from the Zephyr-7B model.

3. **[Gradio](https://github.com/gradio-app/gradio)**  
   - A user-friendly web framework to create interactive demos.
   - Allows the chatbot to display token-by-token responses in a chat UI.

4. **Hugging Face Spaces** (Optional)  
   - For hosting the Gradio app without complex infrastructure setup.

---

## Installation

### Prerequisites

- Python **3.7+** (recommended)
- `pip` or `conda` for installing Python packages