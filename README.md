# Deep Learning Applications 2026–2027

Repository con le soluzioni ai laboratori del corso **Deep Learning Applications** (Università degli Studi di Firenze), anno accademico 2026–2027.

## 📋 Contenuti

| Lab | Titolo | Descrizione | Notebook | Stato |
|-----|--------|-------------|----------|-------|
| **Lab 1** | MLP, reti residuali e CNN | MLP e MLP residuali su MNIST, CNN con e senza connessioni residuali su CIFAR-10, knowledge distillation. Esperimenti tracciati con Weights & Biases. | [`Lab1-CNNs.ipynb`](<Lab1 - CNNs/Lab1-CNNs.ipynb>) | In corso |
| **Lab 3** | Transformers | — | — | Da svolgere |
| **Lab 4** | Out-of-Distribution detection | — | — | Da svolgere |

---

## 🚀 Setup ambiente

### Opzione 1: Conda (consigliata)

**Lab 1 (CNNs):**

```bash
conda env create -f environment-dla.yml
conda activate DLA
```

**Lab 3 e 4 (Transformers e OOD):**

```bash
conda env create -f environment-transformers.yml
conda activate transformers
```

### Opzione 2: pip

```bash
pip install -r requirements.txt
```

### Weights & Biases

Gli esperimenti vengono registrati su [Weights & Biases](https://wandb.ai). Prima di eseguire i notebook effettua il login con la tua API key (da <https://wandb.ai/authorize>):

```bash
wandb login
```

## 💻 Come eseguire

Clona il repository e configura l'ambiente (vedi **Setup ambiente**), poi avvia Jupyter dalla cartella del laboratorio:

```bash
cd "Lab1 - CNNs"
jupyter lab
```

Nel notebook esegui prima la cella **Shared setup**, poi gli esercizi in ordine.

---

## 📝 Note

- I dataset (MNIST, CIFAR-10) **non sono inclusi** nel repository: vengono scaricati automaticamente da `torchvision` nella cartella `data/` alla prima esecuzione.
- Per l'addestramento è consigliata una GPU con supporto CUDA.

---

**Corso**: Deep Learning Applications
**Autore**: Francesco Acciaioli
**Anno accademico**: 2026–2027
