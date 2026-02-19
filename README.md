# Multilingual Generative AI for Culturally Grounded Knowledge

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) 
[![Python](https://img.shields.io/badge/Python-3.x-blue)](https://www.python.org/)

## 🚀 Project Overview
This project is an **implementation and exploration of multilingual generative AI models** focused on improving culturally grounded Natural Language Generation (NLG). The core objective is to develop and test models that can perform effectively and appropriately across diverse cultural and linguistic contexts, moving beyond models primarily trained on English-centric data.

## 🎯 Core Goal (The "Why")
The primary goal is to **develop multilingual generative AI for culturally grounded knowledge**. We aim to address the critical need for models that are robust and relevant when deployed in localized, non-English speaking environments, specifically examining performance in contexts often underrepresented in mainstream AI development.

## 🧠 Model and Architecture
| Component | Details |
| :--- | :--- |
| **Model** | **mT5-small** (Multilingual T5) |
| **Type** | Transformer-based Sequence-to-Sequence Model |
| **Focus** | Multilingual pre-training and fine-tuning for culturally specific text generation tasks. |

## 📊 Dataset and Evaluation
The model's performance was evaluated using a specialized, culturally sensitive benchmark.

*   **Dataset:** **BLEND (Benchmark for Localized, Multilingual, and Culturally Grounded NLG)**.
*   **Purpose:** To validate the model's ability to produce relevant, localized, and culturally appropriate knowledge and text.

## 📈 Key Performance Metrics
The results highlight the model's capabilities and the existing challenges in deploying models across diverse cultural contexts:

*   **US English Data:** **95% Accuracy**
*   **Ethiopia Localized Data:** **$\approx$68% Accuracy**

***Takeaway:*** *While the model performs strongly in high-resource contexts (US), there is a significant performance gap in localized, lower-resource environments (Ethiopia), indicating the need for further fine-tuning and resource development for true cultural grounding.*

## ⚙️ Setup and Installation
Follow these steps to set up the project environment and run the model.

### Prerequisites
*   Python 3.8+
*   [`requirements.txt`](#installation) file with all necessary libraries.

### Installation
1.  Clone the repository:
    ```bash
    git clone [YOUR_GITHUB_URL]
    cd multilingual-generative-ai
    ```
2.  Install the required dependencies:
    ```bash
    # You will need to create this file listing libraries like torch, transformers, etc.
    pip install -r requirements.txt 
    ```

## 💻 Usage
### Running Inference
To run the model on a sample input:
```bash
python run_inference.py --model_path ./checkpoints/best_mt5_model.pt --input_text "Generate a culturally appropriate greeting for [Region/Country]"
