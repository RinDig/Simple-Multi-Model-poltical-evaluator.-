# Multi-Model Political Bias Analyzer Script

This project is a Python script that analyzes political bias in text using multiple AI models: OpenAI's GPT, Anthropic's Claude, and Google's Gemini.

## Features

- Analyzes text for political bias using three different AI models
- Categorizes text as Liberal, Conservative, or Neutral
- Provides explanations for each categorization
- Processes multiple articles from a CSV file

## Requirements

- Python 3.6+
- pandas
- openai
- anthropic
- google-generativeai

## Installation

 Install the required packages:
   ```
   pip install pandas openai anthropic google-generativeai
   ```

Set up API keys:
   - Obtain API keys for OpenAI, Anthropic, and Google AI
   - Replace the placeholder API keys in the script with your actual keys

## Usage

1. Prepare your input data:
   - Create a CSV file named `ModelContext.csv`
   - Include a column named `clean text` (or your preferred column name) containing the articles to analyze

2. Run the script:
   ```
   python political_bias_analyzer.py
   ```

3. If the column name is different from `clean text`, you will be prompted to enter the correct column name.

4. The script will analyze each article using all three AI models and print the results.

## Output

For each article, the script outputs:
- The first 100 characters of the article
- Analysis from OpenAI's model
- Analysis from Anthropic's Claude model
- Analysis from Google's Gemini model

Each analysis includes a categorization (Liberal, Conservative, or Neutral) and a brief explanation.

## Customization

- You can modify the `analyze_text_*` functions to adjust the prompts or parameters for each AI model.
- To use a different OpenAI model (e.g., GPT-4), change the `model` parameter in the `analyze_text_openai` function.

## Note

This script requires valid API keys for OpenAI, Anthropic, and Google AI. Make sure to keep your API keys secure and never share them publicly.
