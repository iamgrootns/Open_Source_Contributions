# Open Source Contributions — Praful Pandey (iamgrootns)

## About Me

Hi, my name is **Praful Pandey**.
I am an AI/ML developer specializing in model training, optimization, and deploying applied machine learning systems for practical applications. I actively contribute to open-source projects in the AI ecosystem and enjoy fixing issues, improving model pipelines, and helping tools become more usable for the community.

I believe open-source collaboration is essential for advancing AI responsibly and making powerful tools accessible to developers worldwide.

---

## My Open Source Contributions

### 1. YingMusic-SVC

Repository: https://github.com/GiantAILab/YingMusic-SVC

This is a project I created and maintain, focused on AI-driven music and voice synthesis experimentation.
It reflects my work in model integration, experimentation, and applied ML tooling.

Upstream fix: [GiantAILab/YingMusic-SVC#5 — Fix undefined variable `bigvgan_cache`](https://github.com/GiantAILab/YingMusic-SVC/pull/5) (merged).

---

### 2. ACE-Step-1.5 Contribution

Pull Request:
https://github.com/ace-step/ACE-Step-1.5/pull/48

I contributed a bug fix and code improvements to the ACE-Step-1.5 project.
This contribution involved debugging model behavior and making changes to improve stability and usability.

---

### 3. coqui-ai-TTS Contribution — Merged

Pull Request:
https://github.com/idiap/coqui-ai-TTS/pull/590

Fixes https://github.com/idiap/coqui-ai-TTS/issues/589 — cached voice lookup failed when `speaker_id` contained a dot. `clone_voice` saves as `slugify(speaker_id).pth` while `load_voice_file` looked up the raw ID, so `my.voice` could never load `my_voice.pth`. Normalized the lookup with `slugify` in both the base mixin (`TTS/utils/voices.py`) and the Bark override (`TTS/tts/models/bark.py`). Reproduced both failure and fix against the real code before opening the PR.

---

### 4. huggingface/optimum Contribution — Ongoing

Pull Request:
https://github.com/huggingface/optimum/pull/2520

Fixes safetensors detection in `try_collect_weight_map` (`optimum/fx/parallelization/utils.py`): the glob pattern list was `["*safetensors", "*.bin"]` while the comparison is against `"*.safetensors"`, so `use_safetensors` was always `False` for safetensors-only models — the wrong index file was read and `weight_files` came back empty. Verified locally with a synthetic sharded-model directory before pushing.

---

## My Open Source Project

### can-you-run-ai

Repository: https://github.com/iamgrootns/can-you-run-ai

"Can You Run It" — for local AI models. An Electron desktop app that detects your hardware, browses Hugging Face, and tells you what actually fits your machine (RAM/VRAM-aware, GGUF-aware). No hardcoded model lists: HF Hub API online, cache works offline.

---

## Focus Areas

* ASR
* Computer Vision
* Model Deployment & Optimization
* Applied ML Systems
* AI Tooling for Developers

---

I plan to continue contributing to open-source AI projects and building tools that help developers and creators work faster with machine learning.

— Praful Pandey
