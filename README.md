# FLAN-T5 PDF QA Fine-Tuning

This project fine-tunes **google/flan-t5-small** using text extracted from a PDF
and synthetic QA pairs generated from that text.

## How It Works
1. Extract text from a PDF
2. Chunk text into overlapping segments
3. Generate QA pairs
4. Train a seq2seq model
5. Run inference

## Usage

### 1. Install dependencies:
pip install -r requirements.txt

### 2. Put your PDF in the same directory and rename it:


### 3. Run training:
python pdf_tuner.ipynb


### 4. Model output + checkpoints will appear in:
results_qa/


## Notes
- Replace the PDF filename in `main.py` if needed.
- Training can take time depending on your GPU.


