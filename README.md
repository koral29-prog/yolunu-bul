# Yolunu Bul

Yolunu Bul, lise öğrencileri ve kariyerinin yönünü araştıran herkes için hazırlanmış, anonim bir kariyer ve üniversite bölümü keşif rehberidir.

## Neler var?

- Kişisel reflekslere odaklanan 12, 24, 36, 48 ve 64 soruluk test
- Cevaplardan çıkan çalışma eğilimlerini açıklayan sonuç ekranı
- 144 meslek için eğitim, çalışma ortamı, talep, maaş aralığı ve ilk deneme bilgileri
- 66 üniversite bölümü için alan, süre ve eğitim yolu filtreleri
- Meslek detayları, favoriler ve üçlü karşılaştırma
- İlerleme, sonuç ve seçimlerin cihazda saklanması
- Mobil uyumlu test akışı ve klavye erişilebilirliği

## Yerelde çalıştırma

```bash
python3 -m http.server 4173
```

Sonra `http://localhost:4173` adresini açabilirsin. Proje build aracı veya backend gerektirmeyen statik HTML, CSS ve JavaScript olarak çalışır.

## Veri yaklaşımı

Meslek verileri yaklaşık ve tarih damgalı aralıklar olarak gösterilir. Detay ekranlarında TÜİK ve YÖK Atlas bağlantıları bulunur; maaş ve talep bilgileri şehir, deneyim ve sektöre göre değişebilir.

## Yayın

Proje GitHub Actions veya özel bir build adımı gerektirmez. `main` dalındaki güncellemeler Netlify üzerinde otomatik yayınlanır.
