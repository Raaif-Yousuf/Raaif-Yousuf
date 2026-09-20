### Hi, I'm Raaif

I'm a computer science student at Vanderbilt (graduating May 2027). I build desktop apps that run AI locally, research tools, and the occasional piece of hardware.

**What I'm working on**

- **[CLAIR Analytics](https://clairanalytics.app)** (private). A local-first desktop app that lets researchers ask questions about their spreadsheets in plain English without the data leaving their machine. React + Tauri frontend, FastAPI backend, DuckDB, Polars, XGBoost, PyTorch, ONNX Runtime.
- **[DNA-Entropy-Graph](https://github.com/Raaif-Yousuf/DNA-Entropy-Graph)**. A Windows app that runs the Evo 2 genomic language model on a cloud GPU and returns per-base entropy tracks for IGV, Geneious, SnapGene and Benchling. Used by researchers in a lab at Vanderbilt University Medical Center.
- **[Wingman](https://github.com/Raaif-Yousuf/Wingman)**. A Windows 11 tray assistant on the Copilot key that looks at your screen and helps, using cloud or local Ollama models. Rust.

**Built at Abako**

- [Abako](https://github.com/Raaif-Yousuf/Abako): a desktop app that runs a national math competition end to end. An Excel question bank goes in, and a 60-question exam with a synced answer key, percentile grading and a printable report card and certificate for every student comes out. Electron, Flask and Python.
- [Abako_emulator](https://github.com/Raaif-Yousuf/Abako_emulator) (private): a pixel-level emulator of the AB-991EX scientific calculator for Windows, macOS and the web. The core is plain TypeScript with no DOM in it, taking key presses through a parser and evaluator onto a 192x63 LCD framebuffer, wrapped in Tauri 2, with 244 golden screen tests so any change that moves a pixel fails the suite.

**Benchmarks and side projects**

- [Zero-Shot-Variant-Effect](https://github.com/Raaif-Yousuf/Zero-Shot-Variant-Effect): a benchmark asking whether DNA language models small enough to run on a laptop CPU can predict variant effects with no training. On 3,644 BRCA1 saturation genome editing SNVs, HyenaDNA and Nucleotide Transformer v2 sit at about 0.45 AUROC against 0.83 for a plain conservation score, with positive controls showing the result is the method and not the harness.
- [AI-Song-lyrics-Generation](https://github.com/Raaif-Yousuf/AI-Song-lyrics-Generation): artist-conditioned lyric generation in PyTorch. An LSTM, a GRU and two transformers on one split and the same 12.3M training tokens, from 2.608 down to 1.892 test bits per character, with an n-gram check showing the best model is also the one that copies most.
- [Syringe_Pump](https://github.com/Raaif-Yousuf/Syringe_Pump): a 3D-printed syringe pump with Arduino firmware.

**Open source**

- tauri-apps/tauri [#16060](https://github.com/tauri-apps/tauri/pull/16060) (open): tauri-bundler cannot build an installer under the Windows SYSTEM account, because it caches its 32-bit NSIS and WiX tools below System32 and WOW64 redirects those tools somewhere they do not exist. The fix keeps them in the project output directory instead.
- tauri-apps/tauri [#16058](https://github.com/tauri-apps/tauri/pull/16058) (open): stop `tauri info` from crashing on package manager versions that are not valid semver.
- dmlc/xgboost [#12583](https://github.com/dmlc/xgboost/pull/12583) (merged): fix `train()` and `cv()` crashing on Windows when a metric is NaN, which MSVC prints as `-nan(ind)`.

**Stack:** Python, TypeScript, C++, Rust, SQL · React, Tauri, FastAPI · DuckDB, Polars, PyTorch, XGBoost · GCP, Docker, GitHub Actions

[LinkedIn](https://linkedin.com/in/raaif1)
