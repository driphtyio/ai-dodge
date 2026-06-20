# AI Dodge 🎯

[![Play Online](https://img.shields.io/badge/Play-Online-00d4ff)](https://aigamingdev.com/games/ai-dodge/)
[![Blog Post](https://img.shields.io/badge/Blog-2D%20Benchmark-ff6b35)](https://aigamingdev.com/blog/llm-benchmark-dodge/)
[![Leaderboard](https://img.shields.io/badge/Leaderboard-LLM%20Scores-00ff87)](https://aigamingdev.com/leaderboard/)

A Phaser.js 3.60 dodge game — **built by 13 different LLMs from the exact same prompt**, ranked and compared.

```
┌──────────────────────────────────────────────┐
│                                              │
│    🔴                    🔴                  │
│              🔵                               │
│    🔴                    🔴         🔴       │
│                                              │
│         🔴                                   │
│                                              │
└──────────────────────────────────────────────┘
     Dodge the red hunters. Survive. Compete.
```

## 🏆 Results — 13 Models

Each model received the same prompt: create a Phaser.js 3.60 dodge game with WASD movement, red chasing enemies, score tracking, wrap-around edges, game over, and R restart.

| Model | Provider | Score | Size | Time |
|-------|----------|-------|------|------|
| Mistral Small ✅ | Mistral API | **95** | 6.3 KB | 12s |
| DeepSeek V4 Flash (0.7) ✅ | DeepSeek Chat | **90** | 15 KB | ~14s |
| owl-alpha ✅ | OpenRouter | **88** | 7.9 KB | 53s |
| DeepSeek V4 Flash (0.4) ✅ | DeepSeek API | **82** | 7.1 KB | 14s |
| GPT-OSS-20B ✅ | Local (Mac Mini) | **78** | 13.5 KB | 23s |
| Nemotron 3 Ultra ✅ | OpenRouter | **76** | 5.1 KB | 86s |
| Qwen 3.5 9B ✅ | Local (Mac Mini) | **74** | 4.6 KB | 190s |
| Llama 3.1 8B ✅ | Local (Mac Mini) | **72** | 6.7 KB | 55s |
| Gemma-4-12b-qat ✅ | Local (Mac Mini) | **70** | 5.2 KB | 281s |
| Gemma-4-12b-coder-fable ✅ | Local (Mac Mini) | **68** | 3.2 KB | 112s |
| DeepSeek V4 Pro ⚠️ | DeepSeek API | **65** | 6.8 KB | 101s |
| Lfm 2.5 8B ❌ | Local (Mac Mini) | — | 25.7 KB | 128s |

[Full Blog Post →](https://aigamingdev.com/blog/llm-benchmark-dodge/)

## 🎮 Play Online

**https://aigamingdev.com/games/ai-dodge/**

- **WASD / Arrow keys** — Move your blue circle
- **Avoid red enemies** — They chase you with seek AI
- **Survive** — Score increases every second
- **R** — Restart after game over

## 📄 Game Files

| File | Model | Source |
|------|-------|--------|
| [`index.html`](index.html) | Main game (reference build) | — |
| [`ai-dodge-deepseek-v4-flash.html`](ai-dodge-deepseek-v4-flash.html) | DeepSeek V4 Flash (interactive, 5 prompts) | [Play](https://aigamingdev.com/games/ai-dodge/deepseek-v4-flash/) |
| [`deepseek-v4-flash-api.html`](deepseek-v4-flash-api.html) | DeepSeek V4 Flash (API, 0.7 temp) | [Play](https://aigamingdev.com/games/ai-dodge/deepseek-v4-flash-api/) |
| [`deepseek-v4-pro.html`](deepseek-v4-pro.html) | DeepSeek V4 Pro | [Play](https://aigamingdev.com/games/ai-dodge/deepseek-v4-pro/) |
| [`gpt-oss-20b.html`](gpt-oss-20b.html) | openai/gpt-oss-20b | [Play](https://aigamingdev.com/games/ai-dodge/gpt-oss-20b/) |
| [`llm-deepseek-v4-flash.html`](llm-deepseek-v4-flash.html) | DeepSeek V4 Flash (0.4 temp) | [Play](https://aigamingdev.com/games/ai-dodge/llm-deepseek-v4-flash/) |
| [`llm-mistral-small.html`](llm-mistral-small.html) | Mistral Small | [Play](https://aigamingdev.com/games/ai-dodge/mistral-small/) |
| [`llm-nemotron-3-ultra.html`](llm-nemotron-3-ultra.html) | Nemotron 3 Ultra | [Play](https://aigamingdev.com/games/ai-dodge/nemotron-3-ultra/) |
| [`llm-owl-alpha.html`](llm-owl-alpha.html) | owl-alpha | [Play](https://aigamingdev.com/games/ai-dodge/owl-alpha/) |
| [`llm-llama-3.1-8b.html`](llm-llama-3.1-8b.html) | Llama 3.1 8B | [Play](https://aigamingdev.com/games/ai-dodge/llama-3.1-8b/) |
| [`llm-gemma-4-12b-coder-fable.html`](llm-gemma-4-12b-coder-fable.html) | Gemma-4-12b-coder-fable | [Play](https://aigamingdev.com/games/ai-dodge/gemma-4-12b-coder-fable/) |
| [`llm-gemma-4-12b-qat.html`](llm-gemma-4-12b-qat.html) | Gemma-4-12b-qat | [Play](https://aigamingdev.com/games/ai-dodge/gemma-4-12b-qat/) |
| [`llm-qwen-3.5-9b.html`](llm-qwen-3.5-9b.html) | Qwen 3.5 9B | [Play](https://aigamingdev.com/games/ai-dodge/qwen-3.5-9b/) |
| [`llm-lfm-2.5-8b.html`](llm-lfm-2.5-8b.html) | Lfm 2.5 8B (empty canvas) | [Play](https://aigamingdev.com/games/ai-dodge/lfm-2.5-8b/) |

## 🧪 Methodology

All variants tested with Playwright headless Chromium + SwiftShader WebGL. Verified: canvas renders, game loop runs, keyboard input works, no JS errors.

Full 3D benchmark also available: see the [3D Space Dodge repo](https://github.com/driphtyio/3d-space-dodge) for 18 models building a Three.js dodge game.

## License

MIT
