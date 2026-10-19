# Gözlemlenebilir Evren — Cosmic Infinity Simulator

Tarayıcıda çalışan, tek dosyalık (Three.js + WebGL) etkileşimli 3B evren simülasyonu.

## Çalıştırma
- `index.html` dosyasını güncel bir tarayıcıda (Chrome, Edge, Firefox, Safari) açın, **veya**
- yerel sunucu ile: `cd evren && python3 -m http.server 8000` → http://localhost:8000

İnternet bağlantısı yalnızca Three.js'in CDN'den (jsDelivr) yüklenmesi için gerekir. Bağlantı yoksa uygulama
anlaşılır bir hata mesajı gösterir. API anahtarı, hesap veya ücretli servis yoktur; tüm veriler dosyanın içindedir.

## Kontroller
| Eylem | Fare | Dokunmatik |
|---|---|---|
| Döndür | Sol tık + sürükle | Tek parmak sürükle |
| Yakınlaş/uzaklaş | Tekerlek | İki parmak kıstır |
| Kaydır | Sağ tık + sürükle | İki parmak sürükle |
| Seç | Tık (veya etikete tık) | Dokun |
| İçine in (alt ölçek) | Çift tık | Çift dokun |
| Üst ölçek | En uzakta tekerleği çevirmeye devam / ⤴ | ⤴ butonu |

Klavye: `Esc` seçimi kapatır, `Backspace` geri, `Boşluk` simülasyonu durdurur.

## Ölçek seviyeleri
Gözlemlenebilir Evren → Laniakea → Yerel Grup → Samanyolu / Andromeda → Güneş Sistemi → Dünya–Ay.
Güneş Sistemi dışındaki tüm seviyeler doğrusal ölçektedir; Güneş Sistemi sıkıştırılmış ölçek kullanır (ekranda belirtilir).

Veri türleri bilgi panelinde rozetle ayrılır: **Gözlemsel veri**, **Model / yaklaşık**, **Temsili görsel**.
