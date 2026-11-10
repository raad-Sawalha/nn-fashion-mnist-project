Image Classification with Deep Learning: Linear, MLP and CNN Comparison

Names: Ra'ad sawalha , sami khzouz, wisam khzouz
IDs: 2310234, 2310062, 2310276
Project goal
Study how neural-network architecture (linear model, MLP, custom CNN, modern CNN / transfer learning) affects classification quality, training time and model size on Fashion-MNIST

## Current status: Phase 1
- [x] Proposal (use case, research question, related work, dataset, split plan)
- [x] Repository and reproducible setup
- [x] Notebook: data loading, stratified split, linear softmax baseline
- [ ] Phase 2: MLP
- [ ] Phase 3: CNNs
- [ ] Phase 4: final model, demo, report

Dataset
Fashion-MNIST (Xiao et al., 2017), 70,000 28x28 grayscale images, 10 classes, MIT license. Downloaded automatically by `torchvision.datasets.FashionMNIST`.

Split: 54,000 train / 6,000 validation (stratified, seed 42) from the official training set. The official 10,000-image test set is used once, in Phase 4.

Setup
```bash
git clone <repo-url>
cd <repo-folder>
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook phase1_linear_baseline.ipynb
```
The notebook also runs on Google Colab (Runtime > Run all). It prints the exact package versions it used.

## Reproducibility
Seed = 42 (Python, NumPy, PyTorch). Split indices are saved to `outputs/split_indices_seed42.npz`. Experiment configurations are saved in `outputs/*_results.json`.

## AI-use disclosure
An AI assistant helped draft the proposal and starter notebook. The team reviewed and understands all code and text.

## References
See the proposal document.
