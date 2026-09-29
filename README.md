# 🚀 Raspberry Pi Compute Module 4 (CM4) Özel Taşıyıcı Kartı (Carrier / IO Board)

Bu proje, Raspberry Pi Compute Module 4 (CM4) için sıfırdan tasarlanmış özel bir taşıyıcı kart (Carrier/IO Board) donanım mimarisini içermektedir. 

Tasarım süreci; yüksek hızlı sinyal yönlendirme (High-Speed Routing), diferansiyel çift (Differential Pair) kuralları, empedans kontrolü gibi donanım mühendisliği prensipleri temel alınarak gerçekleştirilmiştir.


---

## 🛠️ Teknik Özellikler ve Donanım Kapasitesi

### Genel Tasarım (Hardware & PCB)
* **Merkezi Modül:** Raspberry Pi Compute Module 4 (CM4)
* **Soket Yapısı:** Çift Yüksek Yoğunluklu (High-Density) 100-pin Hirose DF40 Konnektörler.
* **Tasarım Aracı:** Altium Designer

### Desteklenen Arayüzler ve Çevre Birimleri
* **Veri / İletişim:** USB 2.0 veriyolu.
* **Ağ (Network):** Gigabit Ethernet with POE
* **Güç Yönetimi (Power Supply):** CM4'ün ihtiyaç duyduğu 5V için 3A güç girişi ve cm4 içinde dahili bulunan 3V3 besleme
* **Genişleme (Expansion):** 40-pin GPIO başlığı ve standart çevre birimi bağlantıları.

---

## 🧠 Mühendislik Yaklaşımı ve Karşılaşılan Zorluklar

Bu kart tasarlanırken basit bir şematik birleştirmeden ziyade, aşağıdaki donanım mühendisliği kuralları sıkı bir şekilde uygulanmıştır:
1. **Empedans Kontrolü (Impedance Control):** USB (90Ω) ve ETHERNET(100Ω) diferansiyel hatları için özel hat kalınlığı (trace width) ve boşluk (clearance) kullanılmıştır
2. **Uzunluk Eşitleme (Length Matching):** Yüksek hızlı sinyallerde faz farkını önlemek amacıyla teknikler kullanılmıştır.


---
