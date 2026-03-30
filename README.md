# 🤖 Posture Analysis System with AI-Based Image Processing and Sensor Integration
Bu proje, bireylerin duruş (postür) bozukluklarını tespit ederek kullanıcıya uyarı vermek amacıyla geliştirilmiş, Yapay Zeka tabanlı görüntü işleme tekniklerini donanım sensörleri ile birleştiren hibrit bir analiz sistemidir.

## 🌟 Öne Çıkan Özellikler
- **Gerçek Zamanlı Duruş Takibi:**  Google_MLkit ile vücut eklem noktalarının tespiti.

- **Sensör entegrasyonu:** İvmeölçer/Jiroskop (MPU6050) verileri ile vücut eğiminin hassas ölçümü.

- **Açı Analizi:** Omuz, boyun ve bel hizasındaki sapmaların matematiksel olarak hesaplanması.

- **Anlık Geri Bildirim:** Hatalı duruş tespit edildiğinde kullanıcıya görsel ve işitsel uyarı sistemi.

- **Veri Kaydı:** Analiz sonuçlarının ileride değerlendirilmek üzere kaydedilmesi.

## 🚀 Kurulum ve Kullanım
- **Repoyu Klonlayın:**

  ```Bash
  git clone https://github.com/serkansvmz/POSTURE-ANALYSIS-SYSTEM-WITH-ARTIFICIAL-INTELLIGENCE-BASED-IMAGE-PROCESSING-AND-SENSOR-INTEGRATION-.git
  ```
  
- **Bağımlılıkları Yükleyin:**
  ```Bash
  dependencies:
  flutter:
    sdk: flutter
  path_provider: ^2.0.15
  camera: ^0.10.0+4
  permission_handler: ^12.0.0+1
  image_picker: ^1.0.8
  google_mlkit_pose_detection: ^0.14.0
  google_mlkit_commons: ^0.11.0
  hive: ^2.2.3
  hive_flutter: ^1.1.0
  http: ^0.13.6
  shared_preferences: ^2.2.2
  ```
  
- **Apk Kurulum Dosyası Oluşturun**

Terminalde:

  ```Bash
  flutter build apk --release
  ```
  ```Bash
  flutter build apk --debug
  ```

## 📊 Çalışma Mantığı
Sistem, kameradan gelen görüntüyü işleyerek eklem noktalarını belirler. Aynı zamanda kullanıcının üzerine yerleştirilen sensörden gelen açı verilerini alır. Bu iki veri kaynağı karşılaştırılarak, kişinin dik durup durmadığı **%90+** doğrulukla analiz edilir.

## 📌Uygulama Arayüz Yapısı
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

# Uygulama Görselleri
<img width="700" height="648" alt="image" src="https://github.com/user-attachments/assets/2a891de7-2083-43d6-8a99-dc7ac8592953" />
<img width="674" height="610" alt="image" src="https://github.com/user-attachments/assets/5faaec6e-aecc-4d03-97bb-679a9124eade" />
<img width="839" height="693" alt="image" src="https://github.com/user-attachments/assets/bb672afe-e255-4e6a-831d-20f88bd6556d" />
<img width="837" height="768" alt="image" src="https://github.com/user-attachments/assets/dcb011ae-fb63-4b7d-b088-3d0cbec5048b" />
<img width="988" height="779" alt="image" src="https://github.com/user-attachments/assets/118d5341-16ff-4a32-aa00-0adb029e3b6f" />








