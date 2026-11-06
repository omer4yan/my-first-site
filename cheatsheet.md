# Shell Komutları Kopya Kağıdı

Yeni başlayanlar için ilk öğrenilmesi gereken 10 temel komut. Bu komutlar Bash'te (Windows'ta Git Bash dahil) çalışır.

---

## 1. `pwd`: Şu an neredeyim?

**Ne yapar:** İçinde bulunduğun klasörün tam yolunu yazdırır.

**Ne zaman:** Terminali açtın, hangi klasörde olduğunu bilmiyorsun ve bir dosya oluşturmadan önce doğru yerde olduğundan emin olmak istiyorsun.

```bash
pwd
# /c/Users/konveyorayd/Documents/Projeler/ilk-projem
```

---

## 2. `ls`: Burada ne var?

**Ne yapar:** Bulunduğun klasördeki dosya ve klasörleri listeler (`-la` ile gizli dosyaları ve ayrıntıları da gösterir).

**Ne zaman:** `.gitignore` dosyasının gerçekten oluşup oluşmadığını görmek istiyorsun. Adı nokta ile başladığı için gizli dosyadır, bu yüzden `-a` gerekir.

```bash
ls -la
```

---

## 3. `cd`: Başka klasöre geç

**Ne yapar:** Çalışma dizinini değiştirir (`cd ..` bir üst klasöre çıkar, `cd ~` ev klasörüne döner).

**Ne zaman:** `deneme` klasöründeki dosyalar üzerinde çalışacaksın ve her seferinde uzun yol yazmak istemiyorsun.

```bash
cd deneme
cd ..        # geri dön
```

---

## 4. `mkdir`: Yeni klasör oluştur

**Ne yapar:** Yeni bir klasör oluşturur (`-p` ile iç içe klasörleri tek seferde açar).

**Ne zaman:** Projene notlarını koyacağın bir `notlar/haftalik` klasörü eklemek istiyorsun.

```bash
mkdir -p notlar/haftalik
```

---

## 5. `touch`: Boş dosya oluştur

**Ne yapar:** Dosya yoksa boş bir dosya oluşturur, varsa yalnızca değiştirilme tarihini günceller.

**Ne zaman:** `deneme/README.md` içinde adı geçen ama aslında olmayan `siir.txt` dosyasını oluşturmak istiyorsun.

```bash
touch deneme/siir.txt
```

---

## 6. `cat`: Dosyanın içini göster

**Ne yapar:** Bir dosyanın içeriğini terminale yazdırır.

**Ne zaman:** Bir editör açmadan `hello.txt` içinde ne yazdığına hızlıca bakmak istiyorsun.

```bash
cat hello.txt
# merhaba
```

---

## 7. `cp`: Kopyala

**Ne yapar:** Dosyayı (ya da `-r` ile klasörü) başka bir yere kopyalar.

**Ne zaman:** README dosyasını değiştirmeden önce, bir şey ters giderse geri dönebilmek için yedeğini almak istiyorsun.

```bash
cp README.md README.yedek.md
```

---

## 8. `mv`: Taşı veya yeniden adlandır

**Ne yapar:** Dosyayı başka bir yere taşır; aynı klasörde kullanırsan adını değiştirir.

**Ne zaman:** `hello.txt` dosyasının adını daha anlamlı bir adla, örneğin `selam.txt` ile değiştirmek istiyorsun.

```bash
mv hello.txt selam.txt
```

---

## 9. `rm`: Sil

**Ne yapar:** Dosyayı (ya da `-r` ile klasörü) kalıcı olarak siler. Geri dönüşüm kutusuna gitmez, dikkatli kullan!

**Ne zaman:** Yukarıda aldığın yedeğe artık ihtiyacın kalmadı ve onu silmek istiyorsun.

```bash
rm README.yedek.md
```

---

## 10. `grep`: Metin ara

**Ne yapar:** Dosyaların içinde bir kelimeyi ya da ifadeyi arar ve eşleşen satırları gösterir (`-r` ile alt klasörlerde de arar).

**Ne zaman:** Projede `siir.txt` dosyasının hangi dosyalarda geçtiğini bulmak istiyorsun.

```bash
grep -r "siir.txt" .
```

---

## Bonus İpuçları

- **Tab** tuşu dosya ve klasör adlarını otomatik tamamlar.
- **↑ / ↓** ok tuşları önceki komutlar arasında gezinir.
- **`komut --help`** bir komutun nasıl kullanıldığını gösterir (ör. `ls --help`).
- **Ctrl + C** çalışan bir komutu durdurur.
