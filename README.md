
# Balık Sınıflandırma Projesi

Bu proje, Akbank Derin Öğrenme Bootcamp için hazırlanmış, TensorFlow ve diğer ilgili kütüphaneler kullanılarak geliştirilen bir Yapay Sinir Ağı (ANN) modeli ile balık türlerini sınıflandırmayı amaçlamaktadır.

## İçindekiler
1. Proje Genel Bakış
2. Gereksinimler
3. Kurulum
4. Veri Seti
5. Model Mimarisi
6. Sonuçlar
7. Kullanım
8. Geliştirme Fikirleri
9. Teşekkürler

## Proje Genel Bakış
Bu proje, balık türlerini sınıflandırmak için bir sınıflandırma sistemi geliştirir. Veri seti, balıkların resimlerini içerir ve model bu görüntüleri işleyerek balığın türünü tahmin eder. Geliştirme ve test için Python ve Jupyter Notebook kullanılmıştır.

## Gereksinimler
- **Pandas**: Veri manipülasyonu ve analizi için
- **NumPy**: Sayısal işlemler için
- **Matplotlib**: Veri görselleştirme için
- **PIL (Pillow)**: Görüntü işleme için
- **TensorFlow**: Yapay sinir ağı modelini oluşturmak ve eğitmek için
- **Scikit-learn (sklearn)**: Veri ön işleme ve veri setini bölmek için
- **Seaborn**: Gelişmiş veri görselleştirme için

## Kurulum
1. Bu projeyi klonlayın:
   ```bash
   [https://github.com/doukansurel/Akbank-Derin-Ogrenme-FishClassification.git]
   ```
2. Gerekli paketleri yükleyin:
   ```bash
   pip install -r requirements.txt
   ```

## Veri Seti
Veri seti, farklı balık türlerine ait etiketlenmiş resimleri içerir. Görseller işlenip yeniden boyutlandırıldıktan sonra modele beslenir. Veri seti, eğitim, doğrulama ve test alt kümelerine bölünmüştür.

## Model Mimarisi
Model, TensorFlow'un Sequential API'si kullanılarak inşa edilmiştir ve şu katmanları içerir:
- Özellik çıkarımı için evrişimsel ve havuzlama katmanları
- Sınıflandırma için yoğun katmanlar
- Aşırı öğrenmeyi (overfitting) önlemek için Dropout katmanları

## Sonuçlar
Model, doğruluk ve kayıp metrikleri ile eğitilmiş ve değerlendirilmiştir. Not defterinde, modelin performansını değerlendirmek için doğru ve yanlış sınıflandırılan görüntüler görselleştirilmiştir.

## Kullanım
Projeyi çalıştırmak için sağlanan Jupyter Not Defterini (`fishclassification.ipynb`) açıp adım adım hücreleri çalıştırın. Gerekli kütüphanelerin yüklü olduğundan emin olun.

## Geliştirme Fikirleri
ANN mimarisi ile alınabilen en yüksek sonuçlardan biri olduğunu düşünüyorum. Daha iyi bir sınıflandırma için elbette daha karmaşık katmanlı modeller oluşturulabilir, Data Augmentation işlemi gerçekleştirilebilir, HiperParametrelerde bazı oynamalar ile alınan sonucun daha üstüne çıkılabilir olduğunu düşünüyorum. Bu projede en çok katmanlardaki nöronlarda ve learning-rate ile değiştirilerek sonuçlarda ciddi bir düzelme gerçekleşmiştir. İnceleyen arkadaşlara şimdiden teşekkürlerimi sunuyorum. İyi çalışmalar...

## Teşekkürler
Bu proje, halka açık veri setleri ve açık kaynaklı araçlar kullanılarak geliştirilmiştir.
@inproceedings {ulucan2020large,
title={Balık Segmentasyonu ve Sınıflandırması İçin Büyük Ölçekli Bir Veri Seti},
author={Ulucan, Oguzhan ve Karakaya, Diclehan ve Turkan, Mehmet},
booktitle={2020 Akıllı Sistemler ve Uygulamalarında Yenilikler Konferansı (ASYU)},
pages={1--5},
year={2020},
organization={IEEE}
}
O.Ulucan, D.Karakaya ve M.Turkan.(2020) Balık segmentasyonu ve sınıflandırması için büyük ölçekli bir veri seti.
Conf. Innovations Intell. Syst. Appli. (ASYU)
