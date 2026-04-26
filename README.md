# Kuantitatif Analiz Terminali
**Borsa İstanbul (BİST) Odaklı Veri Güdümlü Karar Destek Sistemi**

> **Fikri Mülkiyet Bildirimi:** Bu depo, projenin arayüz tasarımını ve sistem mimarisini sergilemek amacıyla hazırlanmış bir tanıtım vitrinidir. Arka planda çalışan puanlama algoritmaları, dinamik risk hesaplama motorları ve veri işleme modelleri ticari nitelik taşıdığı için kaynak kodları kapalı (Private) tutulmaktadır.

---

### Sistem Mimarisi ve Çalışma Prensibi
Bu terminal; Borsa İstanbul (BİST) piyasalarındaki çok boyutlu veri setlerini işleyerek, yatırımcı için rasyonel bir **"Kuantitatif Skor"** üretmek üzere tasarlanmıştır. Sistem; fiyat hareketlerini, hacim karakteristiğini ve piyasa duyarlılığını özgün bir ağırlıklandırma motorunda birleştirerek, öznel yorumlardan arındırılmış bir karar destek mekanizması sunar.

---

### 1. Sistem Katmanları (Arayüz Detayları)

#### Üst Segment: Veri Görselleştirme ve Dinamik Karar Ekranı
Terminalin ana arayüzünde; hisse senedinin anlık fiyat hareketleri, sektörel görece gücü, temel analiz verileri ve algoritmanın ürettiği nihai aksiyon planı (AL / SAT / BEKLE) yer almaktadır. Bu katman, yatırımcının karmaşık piyasa verilerini tek bir bakışta anlamlandırabilmesi için optimize edilmiştir.

[<img width="1919" height="892" alt="1  Ekran Görüntüsü" src="https://github.com/user-attachments/assets/ae013e5e-e1c9-4bf8-a186-2306a47a46bd" />]

#### Alt Segment: Analiz Motoru ve Puanlama Detayları
Bu bölümde sistemin "beyni" olan hesaplama katmanı yer alır. Teknik göstergelerin (Trend, İvme, Para Akışı, Volatilite) matematiksel puanlama sonuçları ve eş zamanlı haber akışından elde edilen duyarlılık çıktıları şeffaf bir hiyerarşiyle listelenir.

[<img width="1919" height="893" alt="2  Ekran Görüntüsü" src="https://github.com/user-attachments/assets/f19567e1-158d-44a3-92c4-3d3f73c07dd1" />]

---

### 2. Uygulama Örneği: DMRGD Kuantitatif Analiz Raporu
Aşağıdaki rapor; sistemin ham piyasa verilerini nasıl işleyip somut bir stratejiye dönüştürdüğünü gösteren canlı bir örnektir. Rapor; dört ana kategorideki puanlama sonuçlarını, matematiksel model çıktısını ve dinamik risk yönetimi (Stop-Loss / Kâr Al) seviyelerini içermektedir.

[<img width="2880" height="2664" alt="DMRGD IS_Denetim_Raporu" src="https://github.com/user-attachments/assets/20aeabcd-9c4d-4013-b9aa-01c21574cd36" />]

> **Not:** Yukarıdaki rapor; teknik veriler, hacim profili ve sentiment analizinin birleşiminden oluşan rasyonel bir özettir ve kesinlikle yatırım tavsiyesi içermez.

---

### Teknik Yetkinlikler
* **Algoritmik Filtreleme:** Piyasadaki sahte sinyalleri (repaint) ve yanıltıcı fiyat hareketlerini elimine eden kalkan mekanizması.
* **Dinamik Risk Yönetimi:** Sabit oranlar yerine, hissenin anlık volatilitesine (ATR) duyarlı, matematiksel olarak optimize edilmiş kâr al ve zarar kes seviyeleri.
* **Hibrit Puanlama:** Teknik verilerle haber akışını korele eden veri güdümlü ağırlıklandırma motoru.

**Kullanılan Teknolojiler:**
`Python` | `Pandas` | `Plotly` | `Streamlit` | `YFinance` | `Kuantitatif Modelleme`
