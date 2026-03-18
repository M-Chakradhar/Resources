# Free LLM API Providers

> A fact-checked, actively maintained list of providers that offer a **free, replenishing** LLM inference API. No credit card required for any of them.

Maintained by **[M Chakradhar](https://www.linkedin.com/in/chakradhar-mantena/)**

![Last Updated](https://img.shields.io/badge/Last%20Updated-March%202026-blue)
![Providers](https://img.shields.io/badge/Providers-17-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## What this is

Most "free AI API" lists include one-time trial credits alongside genuine free tiers without distinguishing between them. A trial credit is a fixed balance that disappears once spent. A free tier is a quota that resets on a schedule and comes back. Every provider on this list falls into the second category.

I went through 100+ providers, tested them, and kept only the ones where the free quota genuinely replenishes. The full breakdown is split into tiers based on reliability, data safety, and how well-documented the free access is.

---

## Tiers

| | Tier | Meaning |
|:-:|------|---------|
| 🟢 | **Tier 1 -- Verified** | Major companies, clear privacy terms, safest to use, no significant caveats |
| 🔵 | **Tier 2 -- Solid** | Legitimate and replenishing, one caveat worth reading |
| 🟡 | **Tier 3 -- Use with awareness** | Free and replenishing, data governance differs from EU/US standards |
| ⚪ | **Tier 4 -- Experimental** | Community projects, no SLA, no data guarantees, personal experiments only |

---

## 🟢 Tier 1 -- Verified Free Tiers

| # | Provider | Category | Models Available | Daily Free Limit | Replenishment | API Key | Notes |
|:-:|----------|----------|:----------------:|:----------------:|:-------------:|---------|-------|
| 1 | [Google AI Studio](https://aistudio.google.com) | Foundational LLM | 3 (Gemini 2.5 Pro, Flash, Flash-Lite) | Flash-Lite: 1,000 req · Flash: 250 req · Pro: 25 req | Daily (midnight PST) | [Get key](https://aistudio.google.com) | Keep billing disabled to stay on the free tier permanently. Disable prompt training in AI Studio settings after signup. |
| 2 | [GroqCloud](https://console.groq.com) | Hardware Accelerated | 10 to 12 (Llama 4, Qwen3, Gemma 3, DeepSeek R1) | ~14,400 req · up to 500K tokens · 30-50 RPM/model | Daily reset + per-minute rolling | [Get key](https://console.groq.com) | Fastest free inference on this list (1,000+ tokens/sec). OpenAI-compatible. Prompts not used for training. |
| 3 | [Cerebras Cloud](https://cloud.cerebras.ai) | Hardware Accelerated | 8 to 10 (Llama 4, Qwen3, DeepSeek R1) | 1,000,000 tokens | Continuous token bucket (refills throughout the day) | [Get key](https://cloud.cerebras.ai) | Highest daily token limit on this list. Prompts not used for training. |
| 4 | [GitHub Models](https://github.com/marketplace/models) | Cloud Native | 30+ (GPT-4o, Llama 4, Phi-4, Mistral Large, Cohere Command R+) | GPT-4o: 50 req · GPT-4o mini: 150 req · Others: 150 req each | Daily (midnight UTC) | [Get key](https://github.com/marketplace/models) | Requires a GitHub account. Each model has an independent daily budget. Best way to access GPT-4o for free. |
| 5 | [Mistral AI](https://console.mistral.ai) | Foundational LLM (EU/GDPR) | 8 (Small, Nemo, Codestral, Devstral) | No monthly cap -- rate-limited RPM/TPM | Continuous per-minute rolling | [Get key](https://console.mistral.ai) | Data in EU data centres, governed by GDPR. Go to Settings > Privacy and disable "Contribute to model improvement" right after signup -- it is on by default. |
| 6 | [NVIDIA NIM](https://build.nvidia.com) | Hardware Accelerated | 100+ (Llama 4, DeepSeek R1, Qwen3, Phi-4, Gemma 3, Nemotron, vision models) | 40 RPM combined across all models · No daily token cap | Continuous per-minute rolling | [Get key](https://build.nvidia.com) | Largest free model catalog on this list. Requires a free NVIDIA Developer account. Non-commercial prototyping only per NVIDIA terms. |
| 7 | [OpenRouter](https://openrouter.ai) | API Aggregator | 30+ free models (DeepSeek V3/R1, Llama 4, Qwen3, Gemma 3) | 50 req/day (no balance) · 1,000 req/day ($10+ loaded, no need to spend it) · 20 RPM | Daily (midnight UTC) | [Get key](https://openrouter.ai) | Append `:free` to model names to use the free tier (e.g. `meta-llama/llama-4-scout:free`). OpenRouter subsidises free model costs directly. |
| 8 | [Cloudflare Workers AI](https://developers.cloudflare.com/workers-ai) | Cloud Native (Edge) | ~30 (Llama 3.1/3.2, Mistral 7B, Gemma) | 10,000 neurons/day (~100-200 responses) | Daily (midnight UTC) | [Get key](https://dash.cloudflare.com) | Bundled with any free Cloudflare account. Uses "neurons" not tokens. Requires Cloudflare Workers runtime to call. |
| 9 | [Hugging Face Serverless](https://huggingface.co/inference-api) | Cloud Native (OSS hub) | Thousands (Llama, Mistral, Qwen, Gemma + fine-tuned community models) | No monthly cap -- rate-limited RPM | Continuous per-minute rolling | [Get key](https://huggingface.co/settings/tokens) | Best for specialised or fine-tuned models unavailable elsewhere. Popular models may queue during peak hours. Not recommended for production by HuggingFace. |
| 10 | [Cohere](https://dashboard.cohere.com) | Foundational LLM | 3 to 4 (Command R, Command R+, Command A) | 1,000 calls/month · 20 calls/min on chat | Monthly (1st of each month) | [Get key](https://dashboard.cohere.com) | Free tier running unchanged for 3+ years. Strong for document Q&A and RAG tasks. Not for commercial or production use on the free key. |

---

## 🔵 Tier 2 -- Solid with a Caveat

| # | Provider | Category | Models Available | Free Limit | Replenishment | Access | Notes |
|:-:|----------|----------|:----------------:|:----------:|:-------------:|--------|-------|
| 11 | [Puter.js](https://developer.puter.com) | Client-side SDK | 100+ | No developer-side cost | Continuous | [Docs](https://developer.puter.com/tutorials/free-llm-api/) | User-pays model: end users fund calls through their own Puter account. Works well for browser-based apps. Not a standard backend API setup. |

---

## 🟡 Tier 3 -- Free but Read the Notes

Data governance on these providers differs from EU or US standards. The free tiers are genuine and replenishing but understand what you are sending before you use them.

| # | Provider | Category | Models Available | Free Limit | Replenishment | Access | Notes |
|:-:|----------|----------|:----------------:|:----------:|:-------------:|--------|-------|
| 12 | [DeepSeek](https://platform.deepseek.com) | Foundational LLM | 3 (V3, R1, Coder) | 1M to 3M tokens/month (non-commercial) | Monthly | [Get key](https://platform.deepseek.com) | Data governed under the provider's local jurisdiction, which differs from EU/US standards. Excellent models. Be mindful of what you send. |
| 13 | [SiliconFlow](https://siliconflow.cn) | Hardware Accelerated | Qwen2.5, DeepSeek V3/R1, GLM-4, Llama 3 | Free-tier models: daily rate-limited access · $1 signup credit (one-time, does not replenish) | Daily (free models only) | [Get key](https://siliconflow.cn) | Same data jurisdiction consideration as above. Only the designated free models have recurring access. The $1 signup credit is not what qualifies this provider. |
| 14 | [Pollinations.AI](https://pollinations.ai) | Community (no signup) | Llama 3.3 70B, Mistral Nemo, DeepSeek, Qwen | No published limit | Continuous | No key required -- call `https://text.pollinations.ai` directly | No formal privacy policy. Community and sponsor funded. Good for anonymous experiments. Do not send sensitive data. |

---

## ⚪ Tier 4 -- Community and Experimental

No guarantees on uptime, data handling, or longevity. Use only for personal experiments with non-sensitive data.

| # | Provider | What it is | Models | Access | Notes |
|:-:|----------|------------|--------|--------|-------|
| 15 | [Petals](https://petals.dev) | Distributed inference across volunteer GPU nodes | Large open models (Llama, Falcon) | `pip install petals` then use the Python client | Open source research project. Prompts pass through volunteer-operated nodes. No data guarantees. |
| 16 | [OllamaFreeAPI](https://github.com/mfoud444/ollamafreeapi) | Public OpenAI-compatible gateway wrapping Ollama | Open models via Ollama | Standard REST endpoint | Single-maintainer hobby project. Free while the maintainer keeps servers running. |
| 17 | [Chutes.ai](https://chutes.ai) | Community-funded GPU inference marketplace | Open-source models | REST API | Operational and legitimate but limited public documentation. Free tier availability may vary. |

---

## Quick comparison

| Provider | Replenishes | Daily Token Budget | Models | Card Required |
|----------|:-----------:|:-----------------:|:------:|:-------------:|
| Google AI Studio | Daily | ~1M (Flash-Lite) | 3 | No |
| GroqCloud | Daily + rolling | ~500K | 10-12 | No |
| Cerebras Cloud | Continuous | 1,000,000 | 8-10 | No |
| GitHub Models | Daily | ~150K | 30+ | No |
| Mistral AI | Continuous | Rate-limited | 8 | No |
| NVIDIA NIM | Per-minute | No cap | 100+ | No |
| OpenRouter | Daily | Varies by model | 30+ free | No |
| Cloudflare Workers AI | Daily | ~10K neurons | ~30 | No |
| Hugging Face Serverless | Continuous | Rate-limited | Thousands | No |
| Cohere | Monthly | 1K calls/month | 3-4 | No |

---

## Using multiple providers together

Every provider on this list uses the OpenAI-compatible API format. Switch providers by changing two lines.

```python
from openai import OpenAI

client = OpenAI(
    base_url="https://api.groq.com/openai/v1",  # change per provider
    api_key="your_key_here"                      # change per provider
)

response = client.chat.completions.create(
    model="llama-4-scout-17b-16e-instruct",
    messages=[{"role": "user", "content": "Hello"}]
)

print(response.choices[0].message.content)
```

**Base URLs:**

| Provider | Base URL |
|----------|----------|
| Google AI Studio | `https://generativelanguage.googleapis.com/v1beta/openai` |
| GroqCloud | `https://api.groq.com/openai/v1` |
| Cerebras Cloud | `https://api.cerebras.ai/v1` |
| GitHub Models | `https://models.inference.ai.azure.com` |
| Mistral AI | `https://api.mistral.ai/v1` |
| NVIDIA NIM | `https://integrate.api.nvidia.com/v1` |
| OpenRouter | `https://openrouter.ai/api/v1` |
| Cloudflare Workers AI | Via Cloudflare Workers SDK |
| Hugging Face Serverless | `https://api-inference.huggingface.co/v1` |
| Cohere | `https://api.cohere.com/compatibility/v1` |

---

## One thing worth knowing

None of the free tiers on this list are meant for production or commercial use. They are for learning, building, and validating ideas. When you have something real that users depend on, that is when it makes sense to move to a paid plan. These tiers exist precisely to get you to that point without spending anything on the way there.

---

## Contributing

If a rate limit has changed, a new free tier has launched, or a provider should be added or removed, open an issue or pull request. Please include a link to the provider's pricing or docs page with any change.

---

## Author

**M Chakradhar**
[LinkedIn](https://www.linkedin.com/in/chakradhar-mantena/) &nbsp;|&nbsp; [GitHub](https://github.com/M-Chakradhar)

If this saved you time, a star on the repo helps others find it.
