# NVIDIA Nemotron Model Reasoning Challenge

**My personal journey with the NVIDIA Nemotron Reasoning Challenge (2026)**

Hi! I'm working on this competition to improve reasoning performance using LoRA adapters on the official Nemotron-3 Nano baseline.

### What I've built so far
- Started with **Qwen2.5-7B-Instruct** as a lighter model to test everything quickly (the full Nemotron was giving me too many memory and setup headaches).
- Created a clean formatting system that teaches the model to always think step-by-step inside `<think>` tags and end with `\boxed{}` — exactly what the competition evaluator looks for.
- Trained a **LoRA adapter** (rank 32) on the full 9,500 training puzzles.
- Successfully created the `submission.zip` file that's ready to upload.

### Project Structure
- `notebooks/01_model_setup_and_training.ipynb` → The main notebook with model loading, data formatting, and training
- `README.md` → This file

### What I learned along the way
The hardest part was actually getting the model to load and run without crashing. Once that was solved, training worked smoothly and the loss dropped nicely.

### Next steps I'm planning
- Switch the base model to the official Nemotron-3 Nano
- Add synthetic data generation and self-correction loops to push accuracy higher
- Train for more steps and try to climb the leaderboard

Everything here is fully reproducible and follows the competition rules (LoRA rank ≤ 32, correct boxed format, etc.).

Made with a lot of patience (and some frustration!) for the NVIDIA Nemotron Model Reasoning Challenge.
