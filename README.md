# Tokenizer Visualizer

A simple Python project for visualizing how different transformer tokenizers break down text into tokens, with each token displayed in a different color.

## Features

- Visualizes tokenization from any Hugging Face transformer model
- Color-coded token display for easy visualization
- Shows vocabulary size of the tokenizer
- Interactive Jupyter notebook interface

## Requirements

- Python 3.7+
- transformers library

## Installation

1. Clone this repository:
```bash
git clone <your-repo-url>
cd tokenizer
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

1. Start Jupyter notebook:
```bash
jupyter notebook
```

2. Open `visualize.ipynb`

3. Modify the `text` and `model_name` variables to experiment with different inputs and tokenizers

4. Run the cells to see the tokenized output with color coding

## Example

```python
text = "Hello, world!"
model_name = "xlm-roberta-base"
show_tokens(text, model_name)
```

This will output each token in a different color, making it easy to see how the tokenizer breaks down the input text.

## Supported Models

Any tokenizer available on Hugging Face Hub can be used, including:
- `bert-base-uncased`
- `bert-base-cased` 
- `xlm-roberta-base`
- `gpt2`
- And many more!

## License

MIT License
