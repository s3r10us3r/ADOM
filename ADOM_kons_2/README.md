# Reprodukcja Mask R-CNN

Wymagane: [uv](https://docs.astral.sh/uv/). Z katalogu tego repozytorium:

```bash
uv sync
uv run jupyter notebook K2_reprodukcja_Mask_RCNN.ipynb
```

Bez GPU: `FORCE_CUDA=0 uv sync` (Detectron2 kompiluje się przy `uv sync`, nie w notatniku). Potem *Run All*.

COCO val2017 jest w `datasets/coco/` (opis w `datasets/README.md`). Obrazy nie są w gicie.

Jeśli brakuje zasobów, pobierz [wagi modelu](https://dl.fbaipublicfiles.com/detectron2/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x/137849600/model_final_f10217.pkl) i zapisz je jako `model_final_f10217.pkl` w katalogu głównym. Zbiór pobierz z [val2017.zip](https://images.cocodataset.org/zips/val2017.zip), a adnotacje z [annotations_trainval2017.zip](https://images.cocodataset.org/annotations/annotations_trainval2017.zip); rozpakuj je zgodnie z układem opisanym w `datasets/README.md`.
