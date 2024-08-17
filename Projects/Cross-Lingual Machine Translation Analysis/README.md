# Cross-Lingual Machine Translation Analysis

## Overview

This project provides a comprehensive analysis of machine translation models applied to Marathi, Hindi, and English languages. The evaluation focuses on three translation models: Distilled NLLB-200, IndicTrans, and ChatGPT. The goal is to assess their performance on various translation tasks and report the results using BLEU and ROUGE metrics.

## Project Structure

The project directory structure is as follows:

- **`<project_root>/`**
  - **`MarathiHindiEnglish_Translation.ipynb`**: Contains the complete implementation for the analysis, including data preparation, model evaluation, and result generation.
  - **`outputs/`**: Contains all output data and results.
    - **`/chatgptOutputs/`**: Contains translation outputs from the ChatGPT model.
    - **`/IndicTrans/`**: Contains translation outputs from the IndicTrans model.
    - **`/NLLB/`**: Contains translation outputs from the Distilled NLLB-200 model.
    - **`outputs/results/`**: Contains JSON files with BLEU and ROUGE scores for each model.
      - `chatgpt_results.json`
      - `indicTrans_results.json`
      - `NLLB_results.json`
  - **`dataset/`**: Contains dataset files used for evaluation.
    - `test.en`: English dataset file.
    - `test.hi`: Hindi dataset file.
    - `test.mr`: Marathi dataset file.
    - `test_1000_en.txt`: Randomly selected 1000 English sentences.
    - `test_1000_hi.txt`: Randomly selected 1000 Hindi sentences.
    - `test_1000_mr.txt`: Randomly selected 1000 Marathi sentences.

## Datasets

- **Samanantar Benchmark Dataset**: [Download Samanantar Dataset](https://drive.google.com/drive/folders/1hR-8Mc7qQWsZAC-cw-nUqG8_OCqCdq-b)
  - Used for evaluating translations between English, Marathi, and Hindi.
- **Wat2021 Test Dataset**: [Download Wat2021 Dataset](https://drive.google.com/drive/folders/1hR-8Mc7qQWsZAC-cw-nUqG8_OCqCdq-b)
  - Used for calculating BLEU and ROUGE scores.

## Models Evaluated

1. **Distilled NLLB-200**
   - A distilled version of the NLLB-200 model with 600M parameters.
   - Model documentation: [Hugging Face NLLB](https://huggingface.co/docs/transformers/en/model_doc/nllb)

2. **IndicTrans**
   - A model tailored for Indic languages.
   - [Model Repository](https://github.com/AI4Bharat/indictrans)

3. **ChatGPT**
   - Utilized for translation tasks via OpenAI’s text generation API.
   - [API Documentation](https://platform.openai.com/docs/guides/text-generation/chat-completions-api)

## Evaluation Tasks

1. **Translation Tasks**:
   - English to Marathi
   - Hindi to Marathi
   - Marathi to English
   - Marathi to Hindi

2. **Metrics**:
   - **BLEU**: Measures the precision of n-grams in the translation.
   - **ROUGE**: Measures the recall of n-grams in the translation.

   The metrics are calculated for each model using a subset of 50 sentences from the wat2021 test dataset.

## How to Run

1. **Setup**:
   - Clone this repository and navigate to the project directory.

2. **Execute Notebook**:
   - Open the `MarathiHindiEnglish_Translation.ipynb` file in Jupyter Notebook or JupyterLab.
   - Follow the instructions within the notebook to run the evaluation scripts.
   - The notebook will guide you through loading the models, running the translations, and generating the results.

3. **Results**:
   - Translation outputs are stored in the `outputs/` folder.
   - BLEU and ROUGE scores for each model are available in `outputs/results/` as JSON files.

## Conclusion

This project provides a detailed evaluation of different machine translation models on Marathi, Hindi, and English language pairs, offering insights into their performance and translation quality.

## Contact

For questions or further information, please contact at akashshiv23@iitk.ac.in
