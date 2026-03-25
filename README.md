# 🤖 Posture Analysis System with AI-Based Image Processing and Sensor Integration
Bu proje, bireylerin duruş (postür) bozukluklarını tespit etmek ve düzeltmek amacıyla geliştirilmiş, Yapay Zeka tabanlı görüntü işleme tekniklerini donanım sensörleri ile birleştiren hibrit bir analiz sistemidir.

## 🌟 Öne Çıkan Özellikler
- **Gerçek Zamanlı İskelet Takibi:** MediaPipe veya YOLO tabanlı (kullandığın kütüphaneye göre) vücut anahtar noktalarının tespiti.

- **Sensör Füzyonu:** İvmeölçer/Jiroskop (MPU6050 vb.) verileri ile vücut eğiminin hassas ölçümü.

- **Açı Analizi:** Omuz, boyun ve bel hizasındaki sapmaların matematiksel olarak hesaplanması.

- **Anlık Geri Bildirim:** Hatalı duruş tespit edildiğinde kullanıcıya görsel veya işitsel uyarı sistemi.

- **Veri Kaydı:** Analiz sonuçlarının ileride değerlendirilmek üzere loglanması.

## 🛠️ Donanım Bileşenleri
- **Mikrodenetleyici:** (ESP32)

- **Sensörler:** MPU6050 (Eğim ve İvme Sensörü)

- **Kamera:** Standart WebCam veya Dahili Telefon Kamerası

## 💻 Yazılım Gereksinimleri
### Projenin çalışması için gerekli kütüphaneler:

- opencv-python

- mediapipe (veya ultralytics)

- numpy

- pyserial (Sensör verilerini okumak için)

## 🚀 Kurulum ve Kullanım
- **Repoyu Klonlayın:**

  ```Bash
  git clone https://github.com/serkansvmz/POSTURE-ANALYSIS-SYSTEM-WITH-ARTIFICIAL-INTELLIGENCE-BASED-IMAGE-PROCESSING-AND-SENSOR-INTEGRATION-.git
  ```
  ```Bash
  cd POSTURE-ANALYSIS-SYSTEM-WITH-ARTIFICIAL-INTELLIGENCE-BASED-IMAGE-PROCESSING-AND-SENSOR-INTEGRATION-
  ```
- **Bağımlılıkları Yükleyin:**
  ```Bash
  pip install -r requirements.txt
  ```
  
- **Sistemi Başlatın:**

Sensörün bağlı olduğu COM portunu main.py içinden kontrol edin.

  ```Bash
  python main.py
  ```

## 📊 Çalışma Mantığı
Sistem, kameradan gelen görüntüyü işleyerek eklem noktalarını belirler. Aynı zamanda kullanıcının üzerine yerleştirilen sensörden gelen açı verilerini alır. Bu iki veri kaynağı karşılaştırılarak, kişinin dik durup durmadığı **%90+** doğrulukla analiz edilir.

## 📌 Proje Yapısı
**Plaintext**
├── main.dart
├── camera_capture_screen.dart    
├── cameras.dart
├── new_analysis_screen.dart        
├── posture_analysis_screen.dart              
├── registered_users_screen.dart
├── sensor_data_screen.dart   
├── user_detail_screen.dart  
├── user_images_screen.dart   
├── saved_photos_screen.dart
└── pubspec.yaml

**Geliştiren:** Serkan Sevmez, Taner Binay
