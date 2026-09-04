## IEEE PQ DATASET

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
  - Techniques: yes infusion, yes early stopping  
  

- **`new copy.ipynb  or optimal_nonadapted`**  
  - Model: Generic DistilBERT  
  - Training: K-Fold Cross Validation  
  - Techniques: No infusion, yes early stopping  
  - 🧪 Baseline result for comparison
---

### 📝 Notes
- **Early stopping** helps prevent overfitting and often improves generalization.
- **Domain infusion** improves model performance on specialized data (e.g., power quality tickets).
- **Multi-text pretraining** offers richer language understanding, improving downstream performance.

**REAL WORLD DATASET Code Repository**: https://github.com/RithikaMathew/ticketModel 


---


## 📚 Citations

Rithika Mathew, Siyuan Du, Mahdi Zarif, Bruce Stephen, James VanZwieten, and Yufei Tang.  
**Power Utility Ticket Processing via Domain Knowledge-Infused Large Language Models**  
*IEEE Access*, 2026 (Under review).

---

## 🙏 Acknowledgments

This work was supported in part by the U.S. National Science Foundation under Grant Nos.  
**CMMI-2145571** and **OAC-2017597**, and the **Florida Power & Light (FPL) Center for Intelligent Energy Technologies (InETech)**.
