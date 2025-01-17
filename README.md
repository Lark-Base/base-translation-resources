# Lark Base Translation Resources

This repository contains translation resources for Lark Base, including a glossary of terms in multiple languages.

## File Structure

- **glossary.json**: The main glossary file containing terms, definitions, and translations in Chinese (`zh`), Traditional Chinese (`zh-TW`), and Japanese (`ja`).
- **README.md**: This file, providing an overview of the repository and instructions for usage.

## How to Use

### Viewing the Glossary
To view the glossary, open the `glossary.json` file. It is structured as follows:
```json
{
  "version": "1.0.0",
  "lastUpdated": "2025-01-17",
  "terms": {
    "term": {
      "partOfSpeech": "noun/verb/adjective/etc.",
      "definition": "Definition of the term",
      "translations": {
        "zh": "Chinese translation",
        "zh-TW": "Traditional Chinese translation",
        "ja": "Japanese translation"
      }
    }
  }
}
```

### Adding or Updating Terms
To add or update terms in the glossary:
1. Open the `glossary.json` file.
2. Add or modify entries under the `terms` section.
3. Ensure translations are provided for Chinese (`zh`), Traditional Chinese (`zh-TW`), and Japanese (`ja`).

### Example: Adding a New Term
```json
{
  "new_term": {
    "partOfSpeech": "noun",
    "definition": "Definition of the new term",
    "translations": {
      "zh": "新术语的中文翻译",
      "zh-TW": "新術語的繁體中文翻譯",
      "ja": "新用語の日本語訳"
    }
  }
}
```

### Updating the Glossary Programmatically
You can use the provided Python script `update_glossary.py` to programmatically update the glossary with new terms from a CSV file. Run the script as follows:
```bash
python3 update_glossary.py
```

## Contributing
If you would like to contribute to this repository, please create a new branch, make your changes, and submit a pull request.

For more information, visit the [GitHub repository](https://github.com/Lark-Base/lark-base-translation-resources).