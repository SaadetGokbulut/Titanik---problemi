Titanic Hayatta Kalma Tahmini Projesi

Bu proje, Titanic felaketindeki yolcuların hayatta kalma durumlarını analiz eden ve tahmin eden bir makine öğrenimi çalışmasını içermektedir.

Proje Özeti

Genel Hayatta Kalma Oranı: Model, 418 yolcudan 152'sinin hayatta kalacağını (%36.4) ve 266'sının hayatta kalamayacağını (%63.6) tahmin etmektedir.
Bu sonuç, eğitim verisindeki %38.4 hayatta kalma oranına oldukça yakındır.

-Temel Bulgular-

Model, "kadınlar ve çocuklar önce" politikasını yansıtmaktadır
Hayatta kalanların çoğunluğu kadın ve çocuklardan oluşmaktadır
1. sınıf yolcuların hayatta kalma olasılığı belirgin şekilde daha yüksektir
Kabin bilgisi olan yolcuların hayatta kalma olasılığı daha yüksektir


-Yaş ve Cinsiyet Etkisi-

Genç kadın yolcuların hayatta kalma ihtimali en yüksek seviyededir
Erkek yolcuların hayatta kalma şansı daha düşüktür
10 yaş altı çocukların hayatta kalma olasılığı yüksektir aileleri tarafından


-Sınıf Etkisi-

1. ve 2. sınıf yolcuların hayatta kalma oranları daha yüksektir
3. sınıf yolcuların hayatta kalma şansı belirgin şekilde daha düşüktür


-Aile Büyüklüğü-

1-3 kişilik küçük ailelerle seyahat edenlerin hayatta kalma şansı daha yüksektir
Yalnız seyahat edenler veya çok kalabalık ailelerin şansı daha düşüktür


-Veri Analizi-

Yaş, SibSp (kardeş/eş sayısı), Parch (ebeveyn/çocuk sayısı), Fare (bilet ücreti) gibi sayısal değişkenler analiz edilmiştir

Korelasyon analizleri yapılmıştır.
Parch-SibSp: 0.41 (Aile bireyleri birlikte seyahat etmiştir)
Parch-Fare: 0.21 (Aile ile seyahat edenler daha yüksek ücret ödemiştir)
Age-SibSp: -0.3 (Yaşlı bireyler daha az kardeş/eş ile seyahat etmiştir)

Modelleme için kullanılan algoritma hem sayısal hem de kategorik değişkenleri işleyebilen CatBoost algoritması kullanılmıştır.Model 1000 iterasyon ile eğitilmiştir

Kategorik Özellikler
Pclass (bilet sınıfı)
Sex (cinsiyet)
Embarked (biniş limanı)

Yeni Özellikler
cabin0: Kabin bilgisi olup olmaması
name_title: Yolcu isimlerinden çıkarılan unvanlar (Mr, Mrs vb.)

Modelin Güçlü Yönleri
Kategorik değişkenleri otomatik işleyebilme.Eksik verilerle başa çıkabilme.Doğrusal olmayan ilişkileri yakalayabilme.

Sonuç olarak,bu analiz, Titanic kazasında hayatta kalma olasılığını etkileyen temel faktörleri aramakta. Model, tarihsel gerçeklerle uyumlu olarak kadınların, çocukların ve üst sınıf yolcuların hayatta kalma şansının daha yüksek olduğunu doğrulamaktadır.
