By leveraging quantized transformer models like Mistral and Mixtral, the system delivers performant, contextually aware responses suitable for both open-domain assistance and specialized domains such as finance, data modeling, and NLP reasoning.
# LocalLLM-ChatUI

**LocalLLM-ChatUI** is a locally hosted, privacy-preserving AI assistant built using Streamlit. It connects seamlessly with large language models (LLMs) such as **Mistral** and **Mixtral** via `llama.cpp` using an OpenAI-compatible API. The application supports streaming multi-turn chat, structured data extraction using Pydantic models, function calling with the Instructor library, and vision-based prompts that combine text and images—all running entirely offline.

## Key Features

- Local, offline-first LLM integration (no external API calls)
- Streamlit-powered interactive chat interface
- Multi-turn memory and system prompts
- Structured response modeling with `pydantic.BaseModel`
- Instructor-style function calling for clean, validated outputs
- Vision-enabled chat for interpreting image + text inputs
- Real-time token streaming for responsive UX

## Supported Models

This interface is compatible with models hosted locally via `llama.cpp`, including:

- `mixtral-8x7b-instruct-v0.1.Q2_K.gguf`
- `mistral-7b-instruct-v0.1.Q4_0.gguf`
- `mistral-function-calling` using `chatml` or `functionary` formats

## Requirements

- Python 3.9+
- `llama-cpp-python` or a running OpenAI-compatible local server
- [llama.cpp](https://github.com/ggerganov/llama.cpp) running on port `8000`
- GPU acceleration optional but recommended

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/LocalLLM-ChatUI.git
   cd LocalLLM-ChatUI

