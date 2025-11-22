# VertigoGames Case 1

https://jupyter.org/try-jupyter/notebooks/index.html?path=notebooks%2FVertigoCase1.ipynb

## Kullanılan Araçlar ve Mantık

1.  **Python** dilinde, **Jupyter Notebook** ortamında gerçekleştirilmiştir.
2.  **Kullanılan Kütüphaneler:** Pandas, NumPy, Matplotlib ve Seaborn.

## Varsayımlar

* **Eksik Retention Değerleri:** Tabloda belirtilmeyen D1, D3, D7, D14 aralarındaki günler için **doğrusal enterpolasyon** kullanılmıştır.
* **Uzun Vadeli Retention:** D14'ten sonraki günler (D15-D30) için Tutma Oranı, son bilinen **D14** değeri olarak kabul edilmiştir.

## Ana Bulgular ve Kararlar

### A/B Testi Temel Sonuçları

* Varyant_A      Temel Gelir (C): 47944256.1  , Satış Etkisi (+D):           8100.0   , Yeni Kaynak Etkisi (+E):        498230.110578
* Varyant_B      Temel Gelir (C): 38313811.8  , Satış Etkisi (+D):           8560.0   , Yeni Kaynak Etkisi (+E):        178636.682738

### Kazanan Varyant
* Analiz sonucunda, uzun vadeli metrik olan 30 günlük **Toplam Kümülatif Gelir** baz alındığında, kazanan varyant: **Varyant [A]** olmuştur.

---

### F Şıkkı Kararı: Hangi İyileştirmeye Öncelik Verilmeli?

En yüksek 30 günlük **toplam gelir artışını** sağlayan ve uzun vadeli, kalıcı bir etkiye sahip olan iyileştirme seçilmelidir.

* **Karar:** **[Geçici 10 Günlük Satış / Kalıcı Yeni Kullanıcı Kaynağı Ekleme]** iyileştirmesine öncelik verilmelidir.
* **Gerekçe:** Bu iyileştirme, tek başına uygulandığında [A veya B] varyantında, diğer seçeneğe göre daha yüksek bir finansal geri dönüş ($ **[En Yüksek Artış Sayısı]** ) sağlamıştır.

### 30 Günlük Kümülatif Toplam Gelir Karşılaştırması
<img width="758" height="489" alt="image" src="https://github.com/user-attachments/assets/6fbd983f-7ebf-43d0-901c-7b14dd0a40be" />

****
