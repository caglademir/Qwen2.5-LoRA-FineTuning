# Qwen2.5-Coder LoRA Fine-Tuning Project

Bu proje, Qwen2.5-Coder-1.5B-Instruct modelini LoRA (Low-Rank Adaptation) tekniği kullanarak özelleştirilmiş kodlama görevleri için eğitmek amacıyla hazırlanmıştır.

## Modeller
Eğitilen modeller Hugging Face üzerine yüklenmiştir:
* **DEEP Model:** [https://huggingface.co/datasets/Naholav/CodeGen-Deep-5K]
* **DIVERSE Model:** [https://huggingface.co/datasets/Naholav/CodeGen-Diverse-5K]

## Eğitim Detayları
Bu projede iki farklı veri seti kullanılmıştır:
1. **DEEP Dataset:** Karmaşık mantık ve reasoning gerektiren problemler.
2. **DIVERSE Dataset:** Çeşitli konularda kodlama problemleri.

### Hyperparameters
* **Base Model:** Qwen/Qwen2.5-Coder-1.5B-Instruct
* **LoRA Rank:** 16
* **Learning Rate:** 2e-4
* **Epochs:** 1

## Dosyalar
* `LoRA_Training_Project.ipynb`: Eğitim için kullanılan Python kodu (Training Script).
* `deep_training_logs.txt`, `diverse_training_logs.txt`: Eğitim sırasındaki loss değerlerini gösteren kayıtlar.
