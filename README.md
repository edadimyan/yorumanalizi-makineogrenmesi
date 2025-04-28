# Makine Öğrenimi Modellerinin Türkçe Yorum Analizindeki Performans Karşılaştırması

Bu çalışmada, Türkçe sosyal medya yorumları üzerinde duygu analizi gerçekleştirilmiş ve farklı metin vektörleştirme teknikleri (TF-IDF ve Word2Vec) ile makine öğrenimi modellerinin (Logistic Regression, SVM, Random Forest, Naive Bayes, KNN ve LSTM) performansları karşılaştırılmıştır. Test sonuçlarına göre TF-IDF tekniği, Word2Vec'e kıyasla daha başarılı bir temsil yöntemi olduğunu kanıtlamıştır. Ayrıca Logistic Regression ve SVM modelleri en yüksek doğruluğu sağlamıştır. Hiperparametre optimizasyonu yapılmaksızın elde edilen sonuçlar, duygu analizi çalışmalarında TF-IDF ile Logistic Regression ve SVM modellerinin öncelikli olarak tercih edilebileceğini göstermektedir.

## Çözüm Dizaynı
Hazırladığımız çözümün akışını adım adım açıklamak gerekirse, süreç aşağıdaki gibi
olacaktır.

### 1. Verinin Hazırlanması
#### ● Yorumların Toplanması:
GPT-4 ve BERT modelleri kullanılarak sosyal medya platformlarından 2000 yorumun
oluşturulması.
#### ● Etiketleme:
Yorumların olumlu, olumsuz ve nötr kategorilerine ayrılarak manuel veya otomatik
olarak etiketlenmesi.
### 2. Verinin Ön İşlemesi
#### ● Metin Temizliği:
Yorumlardan özel karakterler, URL’ler ve anlam taşımayan ifadelerin çıkarılması.
#### ● Dil Düzeltmesi:
Tüm metinlerin küçük harflere dönüştürülmesi ve yazım hatalarının düzeltilmesi.
#### ● Stopword’lerin Çıkarılması:
"ve", "ama" gibi analiz için gereksiz olan kelimelerin kaldırılması.
### 3. Verinin Dizilere Dönüştürülmesi
#### ● Tokenizasyon:
Yorumların kelime veya alt kelime düzeyinde parçalara ayrılması.
#### ● Dizilere Dönüştürme:
Yorumların, makine öğrenmesi modellerine uygun şekilde dizi formatında temsil
edilmesi.
#### ● Embedding:
BERT gömülü temsili kullanılarak yorumların anlam tabanlı vektörlere
dönüştürülmesi.
### 4. Modelleme ve Duygu Sınıflandırması
#### ● Benchmark Modellerinin Kullanımı:
Logistic Regression, Naive Bayes, SVM, Random Forest ve BERT gibi modellerle
sınıflandırma yapılması.
#### ● Eğitim ve Test:
Yorum verisinin eğitim ve test setlerine ayrılarak modellerin eğitilmesi ve doğrulama
yapılması.
### 5. Performans Değerlendirmesi
#### ● Başarım Ölçütleri:
Modellerin doğruluk, F1 skoru, hassasiyet ve duyarlılık gibi metriklerle
değerlendirilmesi.
#### ● Karşılaştırma:
Benchmark modellerinin performanslarının kıyaslanarak en iyi modelin belirlenmesi.
### 6. Raporlama
#### ● Sonuçların Görselleştirilmesi:
Performans metriklerinin grafik ve tablolarla sunulması (ör. doğruluk ve F1 skoru
karşılaştırmaları).
#### ● Değerlendirme:
Modellerin duygu analizi performansı ve sınıflandırmadaki genel başarılarının
yorumlanması.

## Projenin Dosya ve Dizin Yapısı
#### Projenin linki: [Yorum_analizi.ipynb](https://colab.research.google.com/drive/1TDI71Qchp1M6lEtCG6Dv8lyivDzaHs9e?usp=shari)







<img width="311" alt="image" src="https://github.com/user-attachments/assets/9840a0ff-9075-4372-a658-89bde2650b48" />
