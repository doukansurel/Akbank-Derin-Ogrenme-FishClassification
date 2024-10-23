
# Balık Sınıflandırma Projesi

Bu proje, TensorFlow ve diğer ilgili kütüphaneler kullanılarak geliştirilen bir Yapay Sinir Ağı (ANN) modeli ile balık türlerini sınıflandırmayı amaçlamaktadır.

## İçindekiler
1. Proje Genel Bakış
2. Gereksinimler
3. Kurulum
4. Veri Seti
5. Model Mimarisi
6. Sonuçlar
7. Kullanım
8. Teşekkürler

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
   git clone https://github.com/kullanici-adi/balik-siniflandirma.git
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

## Teşekkürler
Bu proje, halka açık veri setleri ve açık kaynaklı araçlar kullanılarak geliştirilmiştir. TensorFlow, Pandas ve Scikit-learn geliştiricilerine, bu çalışmayı mümkün kıldıkları için teşekkür ederiz.
