# Natural language processing course: `The Parse Force - Project 7`
## Register-sensitive machine translation with LLMs

This project investigates how large language models (LLMs) handle formality variation in multilingual translation tasks. We analyze translations from English to German and from English to Sloven using different prompt strategies and evaluate the output quality with BLEU scores.

---

## Table of contents
- [Dataset](#-dataset)
- [LLMs](#-LLMs)
- [Prompting Strategies](#-prompting-strategies)
- [Evaluation Method](#-evaluation-method)
- [Results Summary](#-results-summary)
- [Credits](#-credits)
- [License](#-license)

---

## Dataset
- **Fame-MT Corpus**: English-German parallel data annotated for formality
- **Manual Slovene translations**: created by native speakers for this project.
- Total: 60 English source sentences (30 formal, 30 informal), translated into German and Slovene

---

## LLMs
- GPT-4o (ChatGPT)
- DeepSeek
- Gemma 3 27B

Each model was tested using all four prompting strategies

---

## Prompting Strategies
| Type        | Description |
|-------------|-------------|
| Explicit A  | Few-shot with role + clear task instructions |
| Explicit B  | Chain-of-thought reasoning with register identification |
| Implicit A  | Few-shot with examples only, no task description |
| Implicit B  | Zero-shot with minimal instruction |

---

## Evaluation Methods
- **BLEU Scores** using [`sacrebleu`](https://github.com/mjpost/sacrebleu) for lexical overlap

---

## Results Summary
- GPT-4o performed best overall, especially with Explicit B prompts
- Register preservation was inconsistent across models
- Slovene outputs were more sensitive to prompt quality than German

---

## Credits
This project was deeloped as part of the UL-FRI Course "Natural Language Processing" in 2024/2025 by:
- Ines Karažija
- Isabell Furkert
- Lea Vodopivec
- Supervisor: Aleš Žagar

---

## License
This project is for academic/research purposes only. 
  
