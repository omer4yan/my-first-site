# ilk-projem

Öğrenme ve deneme amaçlı oluşturulmuş ilk proje. Üç sayfalık kişisel bir web sitesi, bir komut satırı kopya kağıdı ve küçük deneme dosyaları içerir.

Siteyi görmek için `index.html` dosyasını tarayıcıda aç.

## Proje Yapısı

```
ilk-projem/
├── index.html
├── projects.html
├── hakkinda.html
├── style.css
├── favicon.svg
├── cheatsheet.md
├── hello.txt
├── deneme/
│   ├── README.md
│   └── .gitignore
├── README.md
└── .gitignore
```

## Dosyalar

| Dosya / Klasör | Açıklama |
|----------------|----------|
| `index.html` | Sitenin ana sayfası. |
| `projects.html` | Projeler sayfası: üç proje, durumları ve yol haritaları. |
| `hakkinda.html` | Hakkında sayfası: öğrenme günlüğü, bilinen komutlar, çalışma şekli. |
| `style.css` | Üç sayfanın ortak stil dosyası (renkler, yazı tipleri, açık/koyu tema). |
| `favicon.svg` | Tarayıcı sekmesinde görünen site simgesi. |
| `cheatsheet.md` | Yeni başlayanlar için 10 temel komutun kopya kağıdı. |
| `hello.txt` | "merhaba" yazan örnek metin dosyası. |
| [`deneme/`](deneme/README.md) | Küçük bir deneme klasörü; ayrıntılar kendi README dosyasında. |
| `README.md` | Projeyi tanıtan bu dosya. |
| `.gitignore` | Git'in takip etmeyeceği dosya ve klasörlerin listesi. |

## Git ile Başlangıç

Proje henüz bir Git deposu değil. Sürüm kontrolüne almak için:

```bash
git init
git add .
git commit -m "İlk commit"
```
