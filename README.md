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
@misc{seo2024manwavmanchuasrmodel,
      title={ManWav: The First Manchu ASR Model}, 
      author={Jean Seo and Minha Kang and Sungjoo Byun and Sangah Lee},
      year={2024},
      eprint={2406.13502},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2406.13502}, 
}
```
