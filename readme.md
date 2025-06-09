## Model Training Descriptions and Results

### 🔍 DistilBERT Variants

- **DistilBERT Enhanced**:  
  Pretrained on **many power quality txtbooks**, but not fine-tuned for classification.

- **DistilBERT PQMLM**:  
  Pretrained on a **single power quality txtbook**, without classification fine-tuning.

---

### 📊 Results Overview

- **`new.ipynb or optimal`**  
  - Model: `DistilBERT Enhanced` 
  - Training: K-Fold Cross Validation  
  - Techniques: yes adaptation, yes early stopping  
  

- **`new copy.ipynb  or optimal_nonadapted`**  
  - Model: Generic DistilBERT  
  - Training: K-Fold Cross Validation  
  - Techniques: No adaptation, yes early stopping  
  - 🧪 Baseline result for comparison
---

### 📝 Notes
- **Early stopping** helps prevent overfitting and often improves generalization.
- **Domain adaptation** improves model performance on specialized data (e.g., power quality tickets).
- **Multi-text pretraining** offers richer language understanding, improving downstream performance.

