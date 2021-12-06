# mt_augment_pos
Machine Translation Data Augmentation Methods Maintaining Part of Speech


# files and descriptions

- notebooks to train models:
  - `TrainLSTM.ipynb`: all LSTM methods excluding sequence matching methods
  - `.`: LSTM sequence matching methods
  - `TrainTransformer.ipynb`: all Transformer methods
  - `LanguageModel.ipynb`: training the language model used in `LMsample` and `soft` methods
- other notebooks:
  - `BEAM_BLEU.ipynb`: *evaluation*, re-compute BLEU score with beam search, compute POS BLEU score
  - `LM_POS_Experiments.ipynb`: *experiment*, looking at how well the language model matches part of speech
  - `Transformer.ipynb`: *development*, developing and testing the transformer architecture
- functions for transformer models:
  - `trainTF.py`
  - `seq2seqTF.py`
  - `embeddingTF.py`
  - `layersTF.py`
  - `sublayersTF.py`
  - `stacksTF.py`
  - `encoderTF.py`
  - `decoderTF.py`
  - `batchTF.py`
- functions for lstm models:
  - `train.py`
  - `Seq2Seq.py`
  - `EncoderLSTM.py`
  - `DecoderLSTM.py`
- other functions:
  - `train.py`: training loop and translating corpus
  - `load_data.py`: creating and loading pickled datasets and dataloaders
  - `similarity_load_data.py`: .
  - `load_lm.py`: load the language model developed in `LanguageModel.ipynb`