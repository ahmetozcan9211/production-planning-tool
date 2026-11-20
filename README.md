# Üretim Planlama Öneri Aracı

Satış, açık sipariş ve depo stok raporlarını analiz ederek mevcut stoğu siparişlere dağıtan ve yetersiz kalan siparişler için **tarih öncelikli üretim iş emri miktarları** öneren web uygulaması.

> Bu depo bir proje vitrinidir. Kaynak kod paylaşılmamaktadır.

## Nasıl çalışır

1. Yıl başından bugüne satış, açık sipariş ve stok raporları (Excel veya CSV) yüklenir
2. Türkçe ve İngilizce kolon başlıkları otomatik tanınır
3. Stok, sipariş tarihine göre **FIFO** yöntemiyle en eski siparişten başlanarak dağıtılır
4. Karşılanamayan miktarlar ürün bazında toplanır ve öncelik sırasıyla üretim önerisine dönüşür

## Özellikler

- Sürükle-bırak dosya yükleme
- Anlık filtreleme ve özet göstergeler
- Önerilen üretim planını CSV olarak indirme
- Docker ile tek komutla çalıştırma, pytest ile test edilmiş hesaplama motoru

## Teknolojiler

`Python` · `pandas` · `FastAPI` · `HTML/JS` · `pytest` · `Docker`
