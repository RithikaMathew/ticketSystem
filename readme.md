## Model Training Descriptions and Results

### 🔍 DistilBERT Variants

- **DistilBERT Enhanced**:  
  Pretrained on **many power quality txtbooks**, but not fine-tuned for classification.

- **DistilBERT PQMLM**:  
  Pretrained on a **single power quality txtbook**, without classification fine-tuning.

---

### 📊 Results Overview

- **`resultsManyTxt`**  
  - Model: `DistilBERT Enhanced`  
  - Training: Fine-tuned for classification  
  - Techniques: Early stopping used  
  - ✅ Best performance due to broader training and regularization

- **`resultsberta`**  
  - Model: `DistilBERT PQMLM`  
  - Training: Fine-tuned for classification  
  - Techniques: Domain adaptation + Early stopping  
  - 📈 Strong results on domain-specific data

- **`abertresults`**  
  - Model: `DistilBERT PQMLM`  
  - Training: Fine-tuned for classification  
  - Techniques: Domain adaptation  + without early stopping  
  - Epochs: 10  
  - ⚠️ Potential overfitting due to fixed number of epochs

- **`results`**  
  - Model: Generic DistilBERT  
  - Training: K-Fold Cross Validation  
  - Techniques: No adaptation, no early stopping  
  - 🧪 Baseline result for comparison

---

### 📝 Notes
- **Early stopping** helps prevent overfitting and often improves generalization.
- **Domain adaptation** improves model performance on specialized data (e.g., power quality tickets).
- **Multi-text pretraining** offers richer language understanding, improving downstream performance.

