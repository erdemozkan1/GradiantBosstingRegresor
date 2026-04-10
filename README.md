# 🏗️ Concrete Strength Prediction using Gradient Boosting

Bu proje, beton bileşenlerini (çimento, su, kül, yaş vb.) analiz ederek betonun basınç dayanımını (**Compressive Strength**) tahmin etmek amacıyla geliştirilmiştir. Projede makine öğrenmesi algoritmalarından **Gradient Boosting Regressor** kullanılmıştır.

## 📊 Veri Seti Hakkında
Kullanılan veri seti, betonun dayanıklılığını etkileyen ham maddelerin miktarlarını içermektedir.
* **Kaynak:** [Kaggle - Concrete Data](https://www.kaggle.com/datasets/zain280/concrete-data)
* **Hedef Değişken:** `Strength` (MPa - Megapaskal)
* **Özellikler (Features):**
    * **Cement:** Çimento miktarı
    * **Blast Furnace Slag:** Yüksek fırın cürufu
    * **Fly Ash:** Uçucu kül
    * **Water:** Su miktarı
    * **Superplasticizer:** Süper akışkanlaştırıcı
    * **Coarse Aggregate:** Kaba agrega
    * **Fine Aggregate:** İnce agrega
    * **Age:** Gün cinsinden yaş

## 🛠️ Kullanılan Teknolojiler
* **Python 3.x**
* **Pandas & NumPy:** Veri manipülasyonu ve analizi.
* **Scikit-Learn:** Model oluşturma, `train_test_split` ve başarı metrikleri.
* **Matplotlib / Seaborn:** Veri görselleştirme ve korelasyon analizi.

## 🚀 Model ve Performans
Projede regresyon problemleri için oldukça güçlü bir topluluk (ensemble) öğrenme yöntemi olan **Gradient Boosting Regressor** tercih edilmiştir. 

### Model Yapılandırması
Modelin eğitim aşamasında aşağıdaki parametreler üzerinde durulmuştur:
* `n_estimators`: Oluşturulacak zayıf öğrenici (ağaç) sayısı.
* `max_depth`: Ağaçların karmaşıklığını kontrol eden derinlik parametresi.
* `learning_rate`: Her yeni ağacın hatayı düzeltme hızı.

### Başarı Metrikleri
Model performansı aşağıdaki kriterlere göre değerlendirilmektedir:
* **R² Score:** Modelin veriyi açıklama oranı.
* **MAE (Mean Absolute Error):** Tahmin edilen değerler ile gerçek değerler arasındaki mutlak hata ortalaması.

## 💻 Kurulum ve Çalıştırma
Projeyi yerelinizde çalıştırmak için:

1. Depoyu klonlayın:
  ```bash
  git clone [https://github.com/erdemozkan1/GradiantBosstingRegresor.git](https://github.com/erdemozkan1/GradiantBosstingRegresor.git)
  ```

2.Gerekli kütüphaneleri yükleyin:
  ```bash
  pip install pandas scikit-learn matplotlib seaborn
  ```

3. Jupyter Notebook veya herhangi bir IDE ile .ipynb dosyasını çalıştırın.



