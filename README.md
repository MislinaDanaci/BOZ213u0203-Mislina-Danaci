# Python Laboratuvar Görevi: Çıktı Biçimlendirme

## Proje Hakkında
Bu proje, Python programlama dilinde temel konsol çıktısı alma yöntemlerini, kaçış dizilerini (escape sequences) ve metin (string) manipülasyonu tekniklerini uygulamalı olarak pekiştirmek amacıyla hazırlanmış bir laboratuvar çalışmasıdır. Proje kapsamında, tek tırnak (') karakterleri kullanılarak terminal ekranına çeşitli ok şekilleri çizdirilmiş ve aşamalı olarak kod optimizasyonu gerçekleştirilmiştir.

## Öğrenim Hedefleri ve Kullanılan Kavramlar
Bu laboratuvar görevi temel olarak üç ana Python konseptine odaklanmaktadır:
1. Ardışık 'print()' fonksiyonları ile konsol ekranında çok satırlı şekiller oluşturmak.
2. '\n' (yeni satır / newline) kaçış dizisini kullanarak `print()` fonksiyonunun çağrılma sayısını asgari düzeye indirmek ve bellek/işlem verimliliği sağlamak.
3. String (metin) çarpımı ('*' operatörü) kullanarak karakter dizilerini yatay eksende matematiksel olarak çoğaltmak ve döngülere gerek kalmadan simetrik şekiller (yan yana iki ok) elde etmek.

## Geliştirme Aşamaları

### 1. Orijinal Versiyon (Temel Çıktı)
İlk aşamada, ekrana tek bir ok şekli çizdirmek için her satır bağımsız bir 'print()' fonksiyonu içerisine yazılmıştır. Bu yaklaşım, şeklin genel hatlarını belirlemek ve boşluk (indentation) hizalamalarını doğru yapmak için bir taslak görevi görmüştür.

### 2. Yeni Satır Karakteri ('\n') ile Optimizasyon
İkinci aşamada kod refactor edilmiştir (iyileştirilmiştir). Çok sayıda 'print()' fonksiyonu kullanmak yerine, şekli oluşturan metin dizelerinin arasına '\n' karakteri yerleştirilmiş ve tüm şekil tek bir 'print()' komutu ile ekrana basılmıştır. Bu işlem, kod satır sayısını ciddi oranda düşürmüş ve yürütme performansını artırmıştır.

### 3. String Çarpımı ile Şekli Çoğaltma
Son aşamada, ekrana yan yana iki adet ok çizdirilmesi hedeflenmiştir. Bu işlem için manuel olarak uzun boşluklar bırakmak veya satırları kopyalamak yerine, Python'un dinamik metin işleme kapasitesinden faydalanılmıştır. Okun ilgili satırları '"metin" *2' formatında çarpılarak, şekil yatay düzlemde mükemmel bir hizalama ile kopyalanmıştır.

## Kurulum ve Çalıştırma
Bu projeyi çalıştırmak için sisteminizde Python 3.x sürümünün yüklü olması yeterlidir. Ekstra bir kütüphane veya bağımlılık (dependency) gerektirmez.

Kodu çalıştırmak için terminal veya komut satırında dosyanın bulunduğu dizine giderek aşağıdaki komutu çalıştırabilirsiniz:

'python_nokta_ok_lab.py'

(Not: Çalıştırma ortamınıza göre komut 'python3_nokta_ok_lab.py' olarak değişiklik gösterebilir. IDE üzerinden çalıştırıyorsanız doğrudan "Run" seçeneğini kullanabilirsiniz.)
