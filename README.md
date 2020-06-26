# Doxygen Çalışma Notlarım
Doxygen yazılım dokümantasyon programı çalışma notlarım. 

# Faydalı Linkler
|||
|---|---|
|Doxygen İndir|http://www.doxygen.nl/download.html|
|Doxygen Örnekler|http://www.doxygen.nl/projects.html|
|Faydalı Eğitim - 1|https://www.youtube.com/watch?v=44Ja2X_fzv4|
|Faydalı Eğitim - 2|https://www.youtube.com/watch?v=LZ5E4vEhsKs|
|Faydalı Eğitim - 3 (Farklı Bir Dokümantasyon Uygulaması İçin)|https://www.youtube.com/watch?v=b4iFyrLQQh4|
|grafikler için|https://mcuoneclipse.com/2012/06/25/5-best-eclipse-plugins-1-eclox-with-doxygen-graphviz-and-mscgen/|

---
## Yükleme 
 - Linux ortamında yükleme yapmak için.
 ```
 sudo apt-get install doxygen
 ```
---
 ## Konfigürasyon Dosyası Oluşturma
 - Yükleme işlemi yapıldıktan sonra projenin bulunduğu dizinde bir adet konfigürasyon dosyası oluşturarak doxygen ayarlarını bununiçinde yapmamız gerekiyor.
 ```
 doxygen -g 
 ```
 - Tabiki konfigürasyon dosyalarının içerisinde bir takım değişiklikler yapmak gerekiyor. Bunlardan başlıcaları ve en öenmlileri
 
 ```
 #Projenin adı yazılmalı
 PROJECT_NAME     = "YENI PROJE"
 
 # Dokümanları çıkarılacağı klasör
 OUTPUT_DIRECTORY = doc
 
 WARNINGS         = YES
 
 # Kodların buluğunduğu klasörler
 INPUT            = src inc
 
 # İncelenecek kodlar.
 FILE_PATTERNS    = *.cpp *.h *.c
  
 EXTRACT_ALL = YES
 
 EXTRACT_PRIVATE = YES
 
 EXTRACT_PACKAGE = YES
 
 EXTRACT_STATIC = YES
 
 # Dosyaların çıkartılacağı adres
 OUTPUT_DIRECTORY = doc
 
 # Eger Dot yazilimi yuklu ise
 HAVE_DOT = YES
 
 ```
 
 - Gereklli olan kofigurasyonlar yapıldıktan sonra asagida bulunan komut çalıştırılır.
 
 ```
 doxygen <config-file>
 ```
 
 
 
