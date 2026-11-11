# Reprodukcja Mask R-CNN

Wymagane: [uv](https://docs.astral.sh/uv/). Z katalogu tego repozytorium:

```bash
uv sync
uv run jupyter notebook K2_reprodukcja_Mask_RCNN.ipynb
```

Bez GPU: `FORCE_CUDA=0 uv sync` (Detectron2 kompiluje się przy `uv sync`, nie w notatniku). Potem *Run All*.

COCO val2017 jest w `datasets/coco/` (opis w `datasets/README.md`). Obrazy nie są w gicie.
