# X-Ray Automated Object Detection & Management System

Bu proje, Roketsan staj programı kapsamında, X-ray cihazlarından geçen bagajlardaki elektronik cihazların (Laptop, Tablet) otomatik tespiti ve bir yönetim paneli üzerinden kontrol edilmesi amacıyla geliştirilmiştir.

## Proje Genel Bakış
Proje kapsamında farklı YOLO mimarileri (`YOLOv5`, `YOLOv8`, `YOLOv9`) karşılaştırılmış ve en kararlı performans **YOLOv9 (gelan-c)** modeliyle elde edilmiştir. Görüntü işleme çıktılarının yönetilmesi için **Next.js**, **MongoDB** ve **Tailwind CSS** tabanlı bir admin paneli tasarlanmıştır.

## Repository Yapısı
- **`notebooks/`**: Model eğitim (`train`) ve tahmin (`predict`) süreçlerini içeren Jupyter Notebook dosyaları.
- **`benchmarks/`**: Farklı modellerin ve görüntü boyutlarının (`640px`, `1280px`) karşılaştırmalı performans grafikleri ve analiz sonuçları.
- **`docs/`**: Projenin tüm teknik detaylarını, veritabanı şemasını ve arayüz tasarımlarını içeren kapsamlı staj raporu.

## ⚙️ Teknik Detaylar (YOLOv9)
- **Model:** YOLOv9
- **Img Size:** 640
- **Batch Size:** 16
- **Epochs:** 100
- **Kütüphaneler:** PyTorch, Ultralytics, OpenCV, Roboflow

## 📊 Veri Seti
Projede kullanılan X-ray veri setine Kaggle üzerinden erişebilirsiniz:
[https://www.kaggle.com/datasets/muhammmed/x-ray-object-detection-dataset]

---
*Bu çalışma bir mühendislik stajı projesidir ve savunma sanayiinde görüntü işleme uygulamaları üzerine bir prototip sunmaktadır.*
