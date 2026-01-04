# 🧠 Müşteri Segmentasyonu ve Analizi (K-Means)

Bu proje, bir alışveriş merkezine ait müşteri verileri kullanılarak **gözetimsiz makine öğrenmesi** yöntemleriyle müşteri segmentasyonu yapılmasını amaçlamaktadır.

Amaç; müşterileri benzer davranışlarına göre gruplamak ve bu grupları **pazarlama stratejileri** açısından yorumlamaktır.

---

## 📌 Proje Özeti

* **Problem Türü:** Unsupervised Learning – Clustering
* **Algoritma:** K-Means
* **Veri Seti:** Mall Customers Dataset (Kaggle)
* **Kullanım Alanı:** Pazarlama, CRM, müşteri analitiği

---

<details>
<summary><strong>📦 Kullanılan Kütüphaneler</strong></summary>

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.graph_objs as go
from sklearn.cluster import KMeans
```

* **NumPy:** Matematiksel işlemler
* **Pandas:** Veri işleme
* **Matplotlib & Seaborn:** Görselleştirme
* **Plotly:** Etkileşimli grafikler
* **Scikit-learn:** K-Means algoritması

</details>

---

<details>
<summary><strong>🔍 Veri Seti İncelemesi (EDA)</strong></summary>

Veri seti 200 müşteriden ve 5 değişkenden oluşmaktadır:

* CustomerID
* Gender
* Age
* Annual Income (k$)
* Spending Score (1–100)

**Öne Çıkan Bulgular:**

* Eksik veri yoktur
* Yaş aralığı: 18–70
* Harcama skoru geniş bir dağılıma sahiptir

Bu yapı, kümeleme analizi için oldukça uygundur.

</details>

---

<details>
<summary><strong>📊 Veri Görselleştirme</strong></summary>

EDA sürecinde aşağıdaki görselleştirmeler yapılmıştır:

* Yaş dağılımı
* Yıllık gelir dağılımı
* Harcama skoru dağılımı
* Cinsiyete göre müşteri sayıları
* Değişkenler arası ilişkiler

Bu analizler, müşteri davranışlarını sezgisel olarak anlamayı sağlamıştır.

</details>

---

<details>
<summary><strong>🤖 K-Means Kümeleme Analizi</strong></summary>

### 1️⃣ Yaş & Harcama Skoru ile Segmentasyon

* Dirsek Yöntemi (Elbow Method) kullanıldı
* En uygun küme sayısı: **4**

---

### 2️⃣ Yıllık Gelir & Harcama Skoru ile Segmentasyon

* Pazarlama açısından en kritik analiz
* En uygun küme sayısı: **5**

Bu segmentasyon sayesinde:

* Yüksek gelir – yüksek harcama
* Yüksek gelir – düşük harcama
* Düşük gelir – yüksek harcama

gibi müşteri profilleri netleşmiştir.

---

### 3️⃣ 3 Boyutlu Segmentasyon (Yaş, Gelir, Harcama)

* 3 değişken birlikte kullanılmıştır
* En uygun küme sayısı: **6**
* Plotly ile 3D görselleştirme yapılmıştır

</details>

---

<details>
<summary><strong>💼 İş Perspektifinden Yorum</strong></summary>

Bu proje sayesinde işletmeler:

* Hedefli pazarlama kampanyaları oluşturabilir
* Yüksek potansiyelli müşterileri tespit edebilir
* Müşteri sadakat stratejilerini geliştirebilir
* Pazarlama bütçesini daha verimli kullanabilir

Segmentasyon sonuçları, **veriye dayalı karar alma** sürecine doğrudan katkı sağlar.

</details>

---

## 🎓 Sonuç

Bu çalışma, K-Means algoritmasının gerçek hayat problemlerinde nasıl uygulanabileceğini göstermektedir.

Elde edilen müşteri segmentleri, pazarlama ve müşteri ilişkileri yönetimi açısından **aksiyon alınabilir içgörüler** sunmaktadır.

---

📌 **Not:** Bu proje eğitim amaçlı hazırlanmıştır ve geliştirilmeye açıktır.
