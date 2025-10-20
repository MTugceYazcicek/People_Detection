# People_Detection
# YOLO ile Gerçek Zamanlı Nesne Tespiti

Bu proje, `YOLO_Hazir_Model.ipynb` Jupyter Notebook'u aracılığıyla, hazır eğitilmiş bir YOLOv8 modeli kullanarak bir web kamerasından (webcam) gerçek zamanlı nesne tespiti yapar.

## 🚀 Amaç

Projenin amacı, `ultralytics` kütüphanesini ve OpenCV'yi (`cv2`) kullanarak canlı video akışındaki nesneleri (örneğin, "person" - insan) tanımak ve bu nesneleri bir dikdörtgen içine almaktır.

## 🔔 Özellikler

* Hazır eğitilmiş `yolov8n.pt` modelini kullanır.
* Web kamerasını (`VideoCapture(0)`) açar ve video akışını işler.
* Tespit edilen nesneleri (kodda "person" olarak filtrelenmiş) ekranda bir kutu ile gösterir.
* Bir nesne tespit edildiğinde `winsound` kütüphanesi ile bir alarm sesi çalar.
* 'q' tuşuna basarak video akışını durdurabilirsiniz.
* 'w' tuşuna basarak alarmı manuel olarak kapatabilirsiniz.

## 🛠️ Kurulum ve Kullanım

### Gereksinimler

Projenin çalışması için gerekli olan Python kütüphaneleri `requirements.txt` dosyasında listelenmiştir.

**Not:** Bu proje, alarm sesi için Windows'a özel `winsound` kütüphanesini kullanır. Eğer macOS veya Linux kullanıyorsanız, `winsound` ile ilgili satırları kaldırmanız veya alternatif bir kütüphane kullanmanız gerekebilir.

### Yerel Kurulum

1.  Depoyu klonlayın:
    ```bash
    git clone [https://github.com/KULLANICI_ADINIZ/PROJE_ADINIZ.git](https://github.com/KULLANICI_ADINIZ/PROJE_ADINIZ.git)
    cd PROJE_ADINIZ
    ```

2.  (Önerilir) Bir sanal ortam (virtual environment) oluşturun ve aktifleştirin:
    ```bash
    python -m venv venv
    source venv/bin/activate  # Windows için: venv\Scripts\activate
    ```

3.  Gerekli kütüphaneleri yükleyin:
    ```bash
    pip install -r requirements.txt
    ```

4.  Jupyter Notebook'u başlatın:
    ```bash
    jupyter notebook YOLO_Hazir_Model.ipynb
    ```

5.  Not defterindeki hücreleri çalıştırın. Web kameranız açılacak ve "Video with Object Detection" başlıklı bir pencerede canlı görüntü gösterilecektir.