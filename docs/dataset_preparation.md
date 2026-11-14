# InfraGuard AI - Dataset Preparation

## Dataset

Cracks in the Foundation (CiF)

Official source:
https://huggingface.co/datasets/ibm-research/cif-dataset

License: CDLA Permissive 2.0

## Defect Categories

1. Algae
2. Crack
3. Net-Crack
4. Crack with Precipitation
5. Rust
6. Spalling

## Experimental Dataset

| Split | Images |
|---|---:|
| Training | 500 |
| Validation | 100 |
| Testing | 100 |
| Total | 700 |

Total annotated instances: 853

## Preprocessing

- Hugging Face streaming dataset access
- Reproducible buffer-based shuffling
- RGB image conversion
- COCO annotation conversion
- Bounding box validation
- Polygon validation
- Dataset integrity verification

## Sampling Configuration

- Random seed: 42
- Shuffle buffer: 1024
- Sampling: Approximate streaming shuffle
- Image format: JPEG
- Annotation format: COCO JSON

## Limitations

The current subset is intended for initial development
and pipeline testing. It is not a statistically
representative benchmark of the complete dataset.

The complete original dataset is not redistributed
through this repository.

## Development Status

Milestone 02: Dataset preparation completed,
subject to successful integrity verification.
