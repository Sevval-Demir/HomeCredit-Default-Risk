# Home Credit Default Risk Prediction

Makine Öğrenmesi (BYM447) dersi kapsamında geliştirilen bu projede, bireylerin kredi başvurularına ait finansal ve demografik bilgiler kullanılarak kredi geri ödeme güçlüğü yaşama olasılığının tahmin edilmesi amaçlanmaktadır.

Proje kapsamında farklı makine öğrenmesi algoritmaları incelenecek, modellerin performansları karşılaştırılacak ve tahmin sonuçları çeşitli değerlendirme yöntemleriyle analiz edilecektir.

## Projenin Amacı

Kredi riskinin doğru tahmin edilmesi, finansal kuruluşların risk değerlendirme süreçlerinde önemli bir yere sahiptir. Bu çalışmada, başvuru sahiplerinin özelliklerinden yararlanılarak kredi geri ödeme güçlüğü göstergesi olan `TARGET` değişkeninin tahmin edilmesi hedeflenmektedir.

Projenin temel amaçları:

- Veri setini keşifsel veri analizi (EDA) ile incelemek.
- Eksik değerleri, aykırı değerleri ve sınıf dengesizliğini değerlendirmek.
- Veri ön işleme yöntemlerini uygulamak.
- Farklı makine öğrenmesi algoritmalarını eğitmek ve karşılaştırmak.
- Model performansını uygun sınıflandırma metrikleriyle değerlendirmek.
- Ablation çalışmaları, öğrenme eğrileri ve hata analizi gerçekleştirmek.

## Veri Seti

**Home Credit Default Risk**

- Kaynak: [Kaggle – Home Credit Default Risk](https://www.kaggle.com/competitions/home-credit-default-risk/data)
- Kullanılan dosya: `application_train.csv`
- Gözlem sayısı: 307.511
- Toplam sütun sayısı: 122
- Tahmin hedefi: `TARGET`

### Hedef Değişken

| Değer | Açıklama |
|---|---|
| 0 | Geri ödeme güçlüğü gözlenmeyen başvuru |
| 1 | Geri ödeme güçlüğü gözlenen başvuru |

Veri setindeki hedef değişken, yarışmanın tanımladığı geri ödeme güçlüğü göstergesidir.

## Kullanılan Teknolojiler

- Python 3.11
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Visual Studio Code
- Git & GitHub

## Proje Yapısı

```text
HomeCredit-Default-Risk/
│
├── data/
│   ├── application_train.csv
│   └── HomeCredit_columns_description.csv
│
├── notebooks/
│   └── home_credit_analysis.ipynb
│
├── outputs/
│   ├── figures/
│   ├── tables/
│   └── results/
│
├── report/
│
├── requirements.txt
├── .gitignore
└── README.md
```

> Not: Büyük veri dosyaları GitHub deposuna eklenmemektedir. Veri setini Kaggle üzerinden indirerek `data/` klasörüne yerleştirebilirsiniz.

## Mevcut Çalışma Durumu

- [x] Veri setinin indirilmesi ve incelenmesi
- [x] Veri sözlüğünün incelenmesi
- [x] Değişken açıklamalarının veri setiyle eşleştirilmesi
- [x] Hedef değişken dağılımının incelenmesi
- [x] Eksik değer analizleri
- [x] Sayısal değişkenlerin dağılımlarının incelenmesi
- [x] Aykırı değer analizleri
- [x] Kategorik değişkenlerin dağılımlarının incelenmesi
- [x] Değişkenlerin hedef değişkenle ilişkilerinin incelenmesi
- [ ] Veri ön işleme
- [ ] Eğitim ve test verilerinin ayrılması
- [ ] Baseline modelinin oluşturulması
- [ ] Makine öğrenmesi modellerinin eğitilmesi
- [ ] Model performanslarının karşılaştırılması
- [ ] Hiperparametre optimizasyonu
- [ ] Ablation çalışmaları
- [ ] Öğrenme ve doğrulama eğrileri
- [ ] Hata analizi
- [ ] Sonuçların değerlendirilmesi ve raporlanması

## Kurulum

Projeyi yerel ortamınızda çalıştırmak için:

```bash
git clone https://github.com/Sevval-Demir/HomeCredit-Default-Risk.git
cd HomeCredit-Default-Risk
```

Sanal ortam oluşturun:

```bash
python -m venv .venv
```

Windows üzerinde sanal ortamı etkinleştirin:

```bash
.venv\Scripts\activate
```

Gerekli kütüphaneleri yükleyin:

```bash
pip install -r requirements.txt
```

Kaggle üzerinden indirdiğiniz veri dosyalarını `data/` klasörüne yerleştirin.

Notebook'u çalıştırın:

```bash
jupyter notebook
```

Ardından `notebooks/home_credit_analysis.ipynb` dosyasını açın.

## Değerlendirme Yaklaşımı

Model performanslarının değerlendirilmesinde aşağıdaki metriklerin kullanılması planlanmaktadır:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

Sınıf dengesizliği nedeniyle yalnızca doğruluk oranı üzerinden değerlendirme yapılmayacaktır.

## Akademik Kapsam

Bu çalışma, BYM447 Makine Öğrenmesi dersi kapsamında bireysel dönem projesi olarak yürütülmektedir.

## Veri Seti Kaynağı

Home Credit Default Risk Competition – Kaggle

https://www.kaggle.com/competitions/home-credit-default-risk/data
