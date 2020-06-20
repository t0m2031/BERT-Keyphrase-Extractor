# Keyphrase Extraction using SciBERT (Semeval 2017, Task 10)

Deep Keyphrase extraction using SciBERT.

## Usage

1. Clone this repository and download model from 'https://drive.google.com/drive/folders/1_VD-pRkA3qNAnTegA0b3F7qFIzXCk5RJ?usp=sharing'
2. Add 4 files of downloaded BERT model to model folder of BERT-keyphrase-Extractor 
3. For training, run the command `python train.py --data_dir data/task1/ --bert_model_dir model/ --model_dir experiments/base_model`
4. For eval, run the command, `python evaluate.py --data_dir data/task1/ --bert_model_dir model/ --model_dir experiments/base_model --restore_file best`

## Results

### Subtask 1: Keyphrase Boundary Identification

On test set, I got:

1. **F1 score**: 0.6259
2. **Precision**: 0.5986
3. **Recall**: 0.6558
4. **Support**: 921

### Subtask 2: Keyphrase Classification


|          | Precision | Recall | F1-score | Support |
|----------|-----------|--------|----------|---------|
| Process  | 0.4734    | 0.5207 | 0.4959   | 870     |
| Material | 0.4958    | 0.6617 | 0.5669   | 807     |
| Task     | 0.2125    | 0.2537 | 0.2313   | 201     |
| Avg      | 0.4551    | 0.5527 | 0.4981   | 1878    |

