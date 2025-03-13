# Meyve Sınıflandırma

## Genel Bakış

Bu proje, farklı meyve görüntülerini sınıflandırmak için makine öğrenimi tekniklerini kullanan bir sınıflandırma modelidir. Veri seti, /train dizininde bulunan meyve görüntülerinden oluşmaktadır. Kullanılan modeller şunlardır:

* Destek Vektör Makineleri (SVM)

* K-En Yakın Komşu (KNN)

* Naive Bayes (GaussianNB)

* Modeller, doğruluk oranı, karmaşıklık matrisi ve sınıflandırma raporu kullanılarak eğitilmiş ve değerlendirilmiştir.

## Veri Seti

* Veri seti, /content/drive/MyDrive/Fruit_Classification/archive/train konumunda saklanmaktadır.

* Görüntüler OpenCV kullanılarak işlenmiş ve skimage.transform.resize() ile yeniden boyutlandırılmıştır.

* Veri seti, train_test_split() fonksiyonu ile eğitim ve test olarak ikiye ayrılmıştır.


# Gerekenler

```bash
pip install numpy pandas matplotlib opencv-python tensorflow keras scikit-learn skimage
```

# Performans

| Model       | Doğruluk Oranı | Precision | Recall | F1-Score |
| ----------- | -------------- | --------- | ------ | -------- |
| SVM         | %85.4          | 0.86      | 0.85   | 0.85     |
| KNN         | %80.2          | 0.81      | 0.80   | 0.80     |
| Naive Bayes | %75.8          | 0.76      | 0.76   | 0.75     |
| DensNet     | %68.3          | -         | -      | -        |
| Vision Transformer | %92.37  | 0.92      | 0.92   | 0.9241   |
| CNN         | %80.62         | 0.74      | -      | 0.8065   |

# Data Seti yüksek boyutlu olduğu için yüklemedim. Aşağıda benzer bir DATA'a erişebilirsiniz.
[LINK](https://drive.google.com/file/d/11ZQ0ILbzixNUMwUaNuIzaQgpH5neoHsa/view?usp=sharing)

