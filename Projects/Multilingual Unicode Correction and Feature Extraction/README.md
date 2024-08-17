# Advanced Multilingual Unicode Correction and Linguistic Feature Extraction

## Project Overview

This project focuses on advanced multilingual Unicode correction and linguistic feature extraction from text data. It involves implementing Unicode correction mechanisms, analyzing linguistic features such as unigram and bigram frequencies, and evaluating the impact of different tokenization methods on text data. The primary techniques employed include Unicode correction, tokenization, and detailed frequency analysis.

## Project Structure

The project is organized into Jupyter Notebook files, each addressing a specific aspect of the project:

1. **`Unicode_Correction_Implementation.ipynb`**
   - Implements Unicode correction mechanisms to standardize and correct text data. It includes handling special characters and ensuring consistency across various linguistic components.

2. **`Characters_and_Syllable_Analysis.ipynb`**
   - Extracts and analyzes syllables from the text data. This notebook performs unigram and bigram syllable analysis and calculates their frequencies.

3. **`Tokenization_Analysis_Unigram_Bigram_BPE_mBERT.ipynb`**
   - Evaluates different tokenization methods, including Unigram, BPE (Byte Pair Encoding), mBERT, and white-space tokenization. This notebook performs unigram and bigram frequency analyses for tokens, syllables, and characters.

4. **`Tokenization_Analysis_Unigram_Bigram_IndicBERT.ipynb`**
   - Evaluates IndicBERT tokenization. This notebook performs unigram and bigram frequency analyses for tokens, syllables, and characters.

5. **`results.ipynb`**
   - Provides a comprehensive analysis of linguistic features, including character and syllable levels, across various tokenization methods. This notebook integrates results from previous analyses for a detailed overview.

## Detailed Description

### Unicode Correction

**Implementation**: In `Unicode_Correction_Implementation.ipynb`, a Unicode correction algorithm is implemented to standardize text by addressing variations in linguistic components such as vowels (swar), consonants (vyanjan), and special characters. The algorithm unifies text representations to ensure consistency and correctness.

### Syllable Extraction and Frequency Analysis

**Implementation**: `Characters_and_Syllable_Analysis.ipynb` focuses on extracting syllables from the text. The notebook performs unigram and bigram syllable frequency analyses to understand syllabic patterns in the data. This analysis helps in identifying the distribution and co-occurrence of syllables in different texts.

### Tokenization Analysis

**Implementation**: `Tokenization_Analysis_Unigram_Bigram_BPE_mBERT.ipynb` evaluates multiple tokenization methods:

- **Unigram**: Tokenization by individual characters or words.
- **BPE (Byte Pair Encoding)**: Tokenization using subword units, tested with vocabulary sizes of 1k and 2k.
- **mBERT (Multilingual BERT)**: Tokenization using multilingual BERT with maximum token lengths of 1k and 2k.
- **White-space**: Tokenization based on white-space separation.

**Implementation**: `Tokenization_Analysis_Unigram_Bigram_IndicBERT.ipynb` evaluates multiple tokenization methods:
- **IndicBERT**: Tokenization using IndicBERT with maximum token lengths of 1k and 2k.

The notebooks calculates unigram and bigram frequencies of tokens, syllables, and characters for each tokenizer, comparing their effectiveness and performance in handling multilingual text data.

### Results

**Implementation**: `results.ipynb` integrates results from the other analyses to provide a detailed overview of linguistic features. It includes comprehensive analyses of character and syllable frequencies, bigrams, and tokenization impacts, offering a complete view of linguistic patterns in the text data.


## Datasets

The `corpus` folder contains all datasets used for the analyses in this project. Ensure that the data is properly placed in this folder before running the notebooks.

## Pretrained Models

The project utilizes the following pretrained models for tokenization and embeddings:

- **mBERT (Multilingual BERT)**: A pretrained model for processing multilingual text data.
- **IndicBERT**: A pretrained model designed for Indic languages.

Ensure you have the necessary libraries to load and use these models. The `transformers` library from Hugging Face provides tools for working with these models.

## Prerequisites

To run the notebooks and scripts in this project, you need the following:

- Python 3.x
- Jupyter Notebook
- Required Python libraries:
  - `numpy`
  - `pandas`
  - `scikit-learn`
  - `torch`
  - `transformers`
  - `sentencepiece`
  - `json`

You can install the required libraries using pip:

```bash
pip install numpy pandas scikit-learn torch transformers sentencepiece
