# PerceptronBee 🐝

Basit bir perceptron uygulaması ile 2 boyutlu veriler üzerinde doğrusal sınıflandırma.  
Bu proje Jupyter Notebook (`.ipynb`) formatında hazırlanmıştır.

## Özellikler
- İki boyutlu veri ile perceptron eğitimi
- Adım adım ağırlık güncelleme
- Öğretici amaçlı

## Kullanım
1. Depoyu klonlayın:
```bash
git clone https://github.com/perceptronBee/perceptron.git
cd perceptron

2. Jupyter Notebook'u açın ve hücreleri çalıştırın:
jupyter notebook perceptron.ipynb


## Algoritma Mantığı
# Tahmin
predict = w * x + b

# Aktivasyon (Step Function)
if predict > 0:
    y_pred = 1
else:
    y_pred = 0

# Hata
error = y_true - y_pred

# Ağırlık Güncelleme
w_new = w_old + eta * error * x
b_new = b_old + eta * error
