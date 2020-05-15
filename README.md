# Doxygen Çalışma Notlarım
Doxygen yazılım dokümantasyon programı çalışma notlarım. 

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
 
 
 ```
 
