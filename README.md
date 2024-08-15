# navigator_ship
# Gezgin Gemi Veritabanı

Bu proje, SQLite kullanarak bir gemi yönetim sistemini simüle eden bir Python uygulamasıdır. Uygulama, farklı türde gemilerin, çalışanların ve seferlerin kaydedilmesini, güncellenmesini, silinmesini ve görüntülenmesini sağlar. Uygulama, kullanıcı arayüzü için `tkinter` kütüphanesini kullanmaktadır.

### Gemi Türleri:
- `CRUISE_SHIP`: Yolcu gemisi
- `OIL_SHIP`: Petrol gemisi
- `CONTAINER_SHIP`: Konteyner gemisi

### Çalışan Türleri:
- `CAPTAIN`: Kaptan
- `CREW`: Mürettebat

### Limana İlişkin Sınıflar:
- `HARBOR`: Liman bilgileri
- `VISITED_HARBORS`: Ziyaret edilen limanlar

### Seferler:
- `EXPEDITIONS`: Sefer bilgileri

### Arayüz:
- `Kayıt Ekle`: Yeni kayıt ekler.
- `Kayıt Sil`: Mevcut bir kaydı siler.
- `Kayıt Güncelle`: Mevcut bir kaydı günceller.
- `Tablo Görüntüle`: Bir tabloyu görüntüler.
- `Kapat`: Uygulamayı kapatır.

### Yapı:

#### Sınıflar:
- `SHIP`: Ana gemi sınıfı (Kullanıcı erişemez).
- `CRUISE_SHIP`, `OIL_SHIP`, `CONTAINER_SHIP`: Gemi türleri için alt sınıflar.
- `EMPLOYEE`: Ana çalışan sınıfı (Kullanıcı erişemez).
- `CAPTAIN`, `CREW`: Çalışan türleri için alt sınıflar.
- `HARBOR`, `VISITED_HARBORS`, `EXPEDITIONS`: Liman ve seferlerle ilgili sınıflar.

#### Fonksiyonlar:
- `_construct_main_menu()`: Ana menüyü oluşturur.
- `_construct_menu(action)`: Alt menüyü oluşturur.
- `_handle_input(textBox, sampleTable, action, classType, c)`: Kullanıcıdan veri alır ve ilgili işlevi çağırır.
- `insert_sample(sampleTable, sampleAttrs, classType, c)`: Yeni kayıt ekler.
- `delete_sample(sampleTable, sampleAttrs, classType, c)`: Mevcut kaydı siler.
- `update_sample(sampleTable, sampleAttrs, c)`: Mevcut kaydı günceller.
- `display_table(sampleTable)`: Bir tabloyu görüntüler.

#### Veritabanı Bağlantısı:
- `conn = sql.connect('gezginGemi.db')`: Veritabanı bağlantısını oluşturur.
- `c = conn.cursor()`: Veritabanı imlecini oluşturur.
