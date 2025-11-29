# Qwen2.5-Coder LoRA Fine-Tuning Project

Bu proje, Qwen2.5-Coder-1.5B-Instruct modelini LoRA (Low-Rank Adaptation) tekniği kullanarak özelleştirilmiş kodlama görevleri için eğitmek amacıyla hazırlanmıştır.

## Modeller
Eğitilen modeller Hugging Face üzerine yüklenmiştir:
* **DEEP Model:** [Buraya Hugging Face DEEP Model Linkini Yapıştır]
* **DIVERSE Model:** [Buraya Hugging Face DIVERSE Model Linkini Yapıştır]

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
* `LoRa.ipynb`: Eğitim için kullanılan Python kodu (Training Script).
* `*_logs.txt`: Eğitim sırasındaki loss değerlerini gösteren kayıtlar.
