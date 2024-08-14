# ManWav

This repository provides the Manchu audio data used in [ManWav: The First Manchu ASR Model](https://arxiv.org/pdf/2406.13502).

## Model Usage
```python
from transformers import AutoProcessor, AutoModelForCTC

processor = AutoProcessor.from_pretrained("seemdog/ManWav")
model = AutoModelForCTC.from_pretrained("seemdog/ManWav")
```

## Citation
```
@inproceedings{seo-etal-2024-manwav,
    title = "{M}an{W}av: The First {M}anchu {ASR} Model",
    author = "Seo, Jean  and
      Kang, Minha  and
      Byun, SungJoo  and
      Lee, Sangah",
    editor = "Serikov, Oleg  and
      Voloshina, Ekaterina  and
      Postnikova, Anna  and
      Muradoglu, Saliha  and
      Le Ferrand, Eric  and
      Klyachko, Elena  and
      Vylomova, Ekaterina  and
      Shavrina, Tatiana  and
      Tyers, Francis",
    booktitle = "Proceedings of the 3rd Workshop on NLP Applications to Field Linguistics (Field Matters 2024)",
    month = aug,
    year = "2024",
    address = "Bangkok, Thailand",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2024.fieldmatters-1.2",
    pages = "6--11",
    abstract = "This study addresses the widening gap in Automatic Speech Recognition (ASR) research between high resource and extremely low resource languages, with a particular focus on Manchu, a severely endangered language. Manchu exemplifies the challenges faced by marginalized linguistic communities in accessing state-of-the-art technologies. In a pioneering effort, we introduce the first-ever Manchu ASR model ManWav, leveraging Wav2Vec2-XLSR-53. The results of the first Manchu ASR is promising, especially when trained with our augmented data. Wav2Vec2-XLSR-53 fine-tuned with augmented data demonstrates a 0.02 drop in CER and 0.13 drop in WER compared to the same base model fine-tuned with original data.",
}
```
