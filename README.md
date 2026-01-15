# cellvision

## Requirements

- mamba
- ssh & scp
- access to local junia server

## Setup

1. Create mamba env 

```bash
mamba env create -f env.yml
```

2. Activate env

```bash
mamba activate cellvision
```

3. Récupérer les datasets depuis le serveur

```bash
scp -r student_cellvision@10.40.150.7:Datasets/Electrophysiology/Islet_MEA60_60HexaMEA_MCS/ ./datasets

```
