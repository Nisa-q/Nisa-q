# Proje Düzeni Standardı

## Adlandırma

Yeni depo adlarında küçük harf, ASCII karakterler ve kelimeler arasında tire kullan: `peri-bale`, `rov-control-system`. Amaç belirten kısa isim seç; son, final, yeni2 gibi adlardan kaçın. Profil deposu `Nisa-q` adını korur. Başka projelerden fork edilen depolarda kaynak proje kimliğini koru.

## Dosya düzeni

- Ana tanıtım: kökte `README.md`.
- Ayrıntılı belgeler: ihtiyaç oldukça `docs/`.
- Statik site görselleri: yeni projelerde `assets/images/`, yazı tipleri: `assets/fonts/`; lisansları yanında tut.
- Python: küçük projede `main.py` veya `app.py` kökte kalabilir.
- Flask: `templates/` ve `static/` düzenini koru.
- Mobil uygulama: kullanılan aracın oluşturduğu yapıyı koru.
- Testler: varsa `tests/`.
- Boş klasörler veya aynı dosyanın final/son kopyaları ekleme.

Mevcut dosyaları taşımadan önce HTML/CSS yolları, Python importları, Docker/Jenkins yapılandırmaları ve README bağlantılarını kontrol et. Repo adı değişince yerel Git adreslerini ve yayın bağlantılarını kontrol et. Taşıma, silme ve repo adlandırma değişiklikleri kullanıcı onayıyla yapılır.

## README şablonu

1. Proje adı ve ne yaptığı.
2. Mevcut durum: planlama, prototip veya tamamlanan özellikler.
3. Teknolojiler ve gerekli araçlar.
4. Kurulum ve çalıştırma: gerçek depo adıyla kopyalanabilir komutlar.
5. Kullanım ve varsa gerçek ekran görüntüsü.
6. Dosya düzeni.
7. Test/elle kontrol adımları; yalnızca gerçekten alınmış sonuçlar.
8. Bilinen eksikler ve sonraki adımlar.
9. Kişisel katkı ve varsa lisans/kaynak bilgisi.

## .gitignore

Genel yerel dosyalar: `.env`, `.env.*`, `!.env.example`, `*.log`, `.DS_Store`, `Thumbs.db`.
Python: `.venv/`, `venv/`, `__pycache__/`, `*.py[cod]`, `.pytest_cache/`.
Node.js: `node_modules/`; Next.js için ayrıca `.next/`.
Mobil: teknoloji belli olunca uygun kuralları seç.

Kaynak kodu, bağımlılık listelerini ve kilit dosyalarını sakla. Git'in zaten takip ettiği dosyalar .gitignore eklenince otomatik kaldırılmaz.

## Commit mesajları

Bir kayıt tek bir anlamlı değişikliği anlatsın:

- `docs: kurulum adımlarını düzelt`
- `fix: iletişim formundaki hatayı düzelt`
- `feat: ürün aramasını ekle`
- `chore: geçici dosyaları hariç tut`
- `test: sepet testi ekle`

## Profil vitrini

Çalıştırılabilen, amacı açıklanmış ve gerçek ekran görüntüsü bulunan projeleri öne çıkar. Yeni proje yalnızca yeni olduğu için değil, gösterilebilir hâle geldiğinde üst sıraya alınır.
