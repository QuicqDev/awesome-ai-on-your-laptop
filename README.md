# Awesome AI on Your Laptop

Find local AI apps for document chat, transcription, dictation, image editing and coding, with setup requirements, source links and practical caveats.

**17 curated entries** · [Browse by task](#browse-by-task) · [Suggest a project](https://github.com/QuicqDev/awesome-ai-on-your-laptop/issues/new?template=suggest-project.yml) · [JSON catalog](catalog.json) · [Agent index](llms.txt)

Choose a useful task, compare the setup, then follow the original project. This collection covers desktop apps and a small set of supporting tools for Windows, macOS and Linux. Local execution is configuration-specific; cloud options are called out where relevant.

## Start here

| If you want to... | Explore | Why it belongs |
|---|---|---|
| Chat with a downloaded model | [Jan](projects/jan.md) | A graphical starting point for local model use. |
| Ask questions about documents | [AnythingLLM](projects/anythingllm.md) | A document workspace with configurable providers. |
| Dictate into another app | [OpenWhispr](projects/openwhispr.md) | Hotkey-based voice input with a local mode. |
| Transcribe an existing recording | [Buzz](projects/buzz.md) | A dedicated transcription interface. |
| Enlarge an image | [Upscayl](projects/upscayl.md) | A focused image upscaler; check Vulkan support. |

## What is checked

Entries distinguish documentation review from hands-on testing. The initial collection is **documentation-reviewed**: source material was inspected, but these applications have not all been installed or benchmarked by QuicqDev. Each project card records its sources, review date, requirements and a limitation.

Hardware requirements depend on model, quantization, context length and workload. We do not infer RAM needs from parameter counts. Application code, model weights and optional hosted services can have different licenses or costs. Check the linked upstream terms for the configuration you choose.

## Browse by task

- [Chat and documents](#chat-and-documents)
- [Transcription and dictation](#transcription-and-dictation)
- [Voice generation](#voice-generation)
- [Images and design](#images-and-design)
- [Documents to data](#documents-to-data)
- [Coding and model runners](#coding-and-model-runners)

## Chat and documents

| Project | Useful for | Setup and requirements |
|---|---|---|
| [Jan](projects/jan.md) · [upstream](https://github.com/janhq/jan) | Start with a graphical local chat app. | Windows, macOS or Linux; memory depends on the downloaded model and context size. |
| [AnythingLLM](projects/anythingllm.md) · [upstream](https://github.com/Mintplex-Labs/anything-llm) | Ask questions across a collection of documents. | Desktop build or self-hosted installation; configure the chat and embedding models. |
| [Open WebUI](projects/open-webui.md) · [upstream](https://github.com/open-webui/open-webui) | Use a browser interface with a locally hosted model. | Python or container setup plus a compatible model backend. |
| [Khoj](projects/khoj.md) · [upstream](https://github.com/khoj-ai/khoj) | Connect personal notes to a conversational assistant. | Self-hosted service and a configured model provider. |

## Transcription and dictation

| Project | Useful for | Setup and requirements |
|---|---|---|
| [Buzz](projects/buzz.md) · [upstream](https://github.com/chidiwilliams/buzz) | Turn recordings into searchable text and subtitle files. | Windows, macOS or Linux; download a speech model. CPU and acceleration options vary by backend. |
| [Vibe](projects/vibe.md) · [upstream](https://github.com/thewh1teagle/vibe) | Generate transcripts without wiring together a Python pipeline. | Supported desktop build and downloaded model; inspect GPU backend support for your OS. |
| [OpenWhispr](projects/openwhispr.md) · [upstream](https://github.com/OpenWhispr/openwhispr) | Speak text into the application you are already using. | Windows, macOS or Linux; microphone access and a selected speech model. |
| [whisper.cpp](projects/whisper-cpp.md) · [upstream](https://github.com/ggml-org/whisper.cpp) | Build an offline transcription command or lightweight voice interface. | A downloaded Whisper model and matching build; CPU-only inference and several GPU backends are available. |
| [Karaoke Captions](projects/karaoke-captions.md) · [upstream](https://karaokecaptions.com/) | Turn local video into editable animated captions and MP4, SRT or VTT exports. | Desktop Chrome or Edge recommended for MP4 export; initial app and speech-model download, then local processing. |

## Voice generation

| Project | Useful for | Setup and requirements |
|---|---|---|
| [Piper](projects/piper.md) · [upstream](https://github.com/OHF-Voice/piper1-gpl) | Generate spoken narration from text using a local voice. | Install the engine and a compatible voice model using upstream instructions. |

## Images and design

| Project | Useful for | Setup and requirements |
|---|---|---|
| [Upscayl](projects/upscayl.md) · [upstream](https://github.com/upscayl/upscayl) | Enlarge an image with a simple graphical workflow. | Windows, macOS or Linux; upstream requires a compatible Vulkan GPU and notes limitations for integrated GPUs. |
| [InvokeAI](projects/invokeai.md) · [upstream](https://github.com/invoke-ai/InvokeAI) | Work on generated images with a visual canvas workflow. | A supported installation and image model; consult current model-specific memory and accelerator guidance. |
| [ComfyUI](projects/comfyui.md) · [upstream](https://github.com/Comfy-Org/ComfyUI) | Combine generation and processing steps in a visual graph. | Desktop or Python installation, model files and hardware appropriate to the workflow. |

## Documents to data

| Project | Useful for | Setup and requirements |
|---|---|---|
| [Docling](projects/docling.md) · [upstream](https://github.com/docling-project/docling) | Convert PDFs into structured text before indexing or summarizing them. | Python environment and the model assets required by the chosen conversion pipeline. |

## Coding and model runners

| Project | Useful for | Setup and requirements |
|---|---|---|
| [Aider](projects/aider.md) · [upstream](https://github.com/Aider-AI/aider) | Ask an assistant to edit a version-controlled codebase. | Python, Git and a supported model connection; local use requires a separately running local backend. |
| [Ollama](projects/ollama.md) · [upstream](https://github.com/ollama/ollama) | Serve a local model to a chat UI or Python application. | Windows, macOS or Linux and sufficient resources for the selected model. |
| [llama.cpp](projects/llama-cpp.md) · [upstream](https://github.com/ggml-org/llama.cpp) | Control a local model server and its inference settings directly. | Compatible build and model file; supports CPU and multiple acceleration backends. |

## Frequently asked questions

### Can I use these apps without a paid API key?

Several entries provide local inference after downloading software and models. Optional cloud models or features may require a paid key. Check the project card and upstream configuration rather than treating the whole application as free to run.

### Will these work on an 8 GB or 16 GB laptop?

There is no universal answer. Model size, quantization, context length, input resolution, GPU memory and operating system all matter. The collection links to requirements rather than assigning unsupported memory guarantees. Reproducible hardware reports are welcome.

### Does local AI mean no network traffic?

Not automatically. Downloads, update checks, optional cloud providers and custom extensions can use the network. Use a documented local configuration; this collection has not audited network behavior.

### Are all entries open source?

The collection prioritizes inspectable projects but includes local tools with custom or mixed terms, explicitly noted in their cards. Code licenses and model licenses must be checked separately.

## How to contribute

Add a useful project, correct an outdated entry, or submit a reproducible compatibility report. Edit `catalog.json` and run `python scripts/build.py`; the README, project cards and agent index are generated from that source. See [CONTRIBUTING.md](CONTRIBUTING.md) for selection criteria and the field format.

Automated checks validate the catalog on changes and check external links weekly. A reachable link does not establish that software works, is secure, or fits your hardware. Failed and inconclusive checks need review; metadata checks never advance an editorial review date.

## For agents and search tools

Read the [structured catalog](https://raw.githubusercontent.com/QuicqDev/awesome-ai-on-your-laptop/main/catalog.json), its [schema](catalog.schema.json), or the compact [llms.txt index](https://raw.githubusercontent.com/QuicqDev/awesome-ai-on-your-laptop/main/llms.txt). Each entry has a stable ID, category, use case, prerequisites, caveat, evidence level and source URLs. Cite the upstream project for its capabilities and this collection for editorial comparisons.

`llms.txt` is a navigation aid, not a promise of inclusion in any search engine or model response. Unknown requirements remain unknown; documentation-reviewed entries must not be described as personally tested.

## Related QuicqDev collections

- [Awesome Small AI Apps](https://github.com/QuicqDev/awesome-small-ai-apps) — Practical small-model AI applications and building blocks for OCR, speech, embeddings, browser AI, mobile vision and text extraction.
- [Awesome Open-Source AI Discoveries](https://github.com/QuicqDev/awesome-open-source-ai-discoveries) — Explore creative open-source AI projects for 3D, images, video, music, speech and documents, with upstream examples, setup notes and limitations.

## Maintainers and attribution

Curated by [Ashutosh Mishra](https://github.com/ASH1998) at [QuicqDev](https://github.com/QuicqDev). Follow [@ashu_mi_2](https://x.com/ashu_mi_2) for project discoveries and practical AI experiments.

All linked projects belong to their respective creators. This repository contains original editorial summaries and links; it does not relicense third-party software, model weights or media. No paid placement or affiliate ranking is included.

If this collection helped you find something useful, star it to bookmark it. Use GitHub Watch settings for notifications, or contribute an entry to help the next reader.

Original catalog text and maintenance scripts: [MIT License](LICENSE).
