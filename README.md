# cellvision

## Requirements

- mamba
- ssh & scp
- accès au serveur junia local

## Setup

1. Créer un environnement mamba

```bash
mamba env create -f env.yml
```

2. Activer l'env

```bash
mamba activate cellvision
```

3. Récupérer les datasets normalisés depuis le serveur

```bash
scp -r student_cellvision@10.40.150.7:normalized_datasets normalized_datasets/

```

## Ajouter une dépendance

1. Installer la dépendance

```bash
pip install <dependency>
```

2. Ajouter la dépendance à l'environnement

```bash
mamba env export --from-history > env.yml
```