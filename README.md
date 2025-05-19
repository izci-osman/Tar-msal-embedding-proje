# Tarımsal Karar Destek Sistemi

Bu projede:

- Projede yaklaşık 5000 resim embedding yapılmış ve 10 meyve, sebze esas alınmıştır. Projem bu meyve sebzelerin hastalıklı olup olmadığını anlamakta, hastalıklı ise hastalığını bulmakta ve tedavisi için çözüm yolları üretmektedir. Aynı zamanda bu 10 meyve sebzeye dahil olmayan başka bir bitki resmi eklediğimizde, önceden yüklenen resimlerle bu resmi kıyas yapmakta ve ona en çok benzeyen resmi bulup onun üzreinden bize çıktı verip yorum yapmaktadır.
- Projede LLM ve VLM kullanılmıştır ama VLM doğrudan kullanılmamıştır.Projede doğrudan bir görüntü+metin entegre VLM kullanılmıyor ama CLIP tabanlı embedding karşılaştırması yapılıyor. 
- Görsellerin embedding'leri çıkarılmıştır.
- Kod dosyası: `main.py`
- Embedding arşivi: `Embeddings.rar` (yüklenmiştir)

## Dosyalar

- `main.py`: Embedding yükleme, benzerlik karşılaştırma ve GPT-4 ile etkileşimli konuşma kodları
- `Embeddings.rar`: Tüm embedding verilerinin arşivi
- `.gitignore`: Büyük boyutlu resim dosyaları hariç tutulmuştur
- `2.zip`: Bu dosyada kullandığım çok yönlü açılardan 5000 resim bulunmaktadır

## Kullanım

Projeyi çalıştırmak için:

```bash
python main.py
```

Kullanıcıdan giriş alır, görsellerle benzerlik bulur ve GPT ile etkileşime girer.
