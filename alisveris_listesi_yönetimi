urunBilgileri = [
    {"ürün": "kazak", "adet": 100, "fiyat": 95},
    {"ürün": "gömlek", "adet": 110, "fiyat": 90},
    {"ürün": "pantalon", "adet": 200, "fiyat": 110}
]

def urunEkle(urunBilgileri):
    urunAdi = input("Eklemek istediğiniz ürünün adını yazınız: ")
    adet = int(input("Eklemek istediğiniz ürünün adedini yazınız: "))
    fiyat = int(input("Eklemek istediğiniz ürünün fiyatını yazınız: "))
    yeniUrun = {"ürün": urunAdi, "adet": adet, "fiyat": fiyat}
    urunBilgileri.append(yeniUrun)
    print(urunAdi + " isimli ürün " + str(adet) + " adet ve " + str(fiyat) + " fiyatı ile eklendi.")

def urunGuncelle(urunBilgileri):
    urunAdi = input("Bilgilerini güncellemek istediğiniz ürünün adını yazınız: ")
    for urun in urunBilgileri:
        if urun["ürün"] == urunAdi:
            yeniUrunAdedi = int(input("Yeni ürün adedini giriniz: "))
            yeniUrunFiyati = int(input("Yeni ürün fiyatını giriniz: "))
            urun["adet"] = yeniUrunAdedi
            urun["fiyat"] = yeniUrunFiyati
            print(urunAdi + " isimli ürünün yeni adedi: " + str(yeniUrunAdedi) + ", yeni fiyatı: " + str(yeniUrunFiyati) + " olarak güncellendi.")
            return
    print(urunAdi + " isimli ürün bulunamadı.")

def urunSil(urunBilgileri):
    urunAdi = input("Silmek istediğiniz ürünün adını yazınız: ")
    for urun in urunBilgileri:
        if urun["ürün"] == urunAdi:
            urunBilgileri.remove(urun)
            print(urunAdi + " isimli ürün silindi.")
            return
    print(urunAdi + " isimli ürün bulunamadı.")

def listeGoruntuleme(urunBilgileri):
    for urun in urunBilgileri:
        print("Ürün: " + urun["ürün"] + ", Adet: " + str(urun["adet"]) + ", Fiyat: " + str(urun["fiyat"]))

def toplamMaliyet(urunBilgileri):
    toplam = 0
    for urun in urunBilgileri:
        toplam += urun["fiyat"] * urun["adet"]
    return toplam

while True:
    print("\nAlışveriş Listesi Yönetim Sistemine Hoş Geldiniz")
    print("1. Ürün Ekleme")
    print("2. Ürün Güncelleme")
    print("3. Ürün Silme")
    print("4. Listeyi Görüntüleme")
    print("5. Toplam Maliyeti Hesaplama")
    print("6. Çıkış")

    secim = int(input("Lütfen yapmak istediğiniz işlemi seçiniz (1-6): "))

    if secim == 1:
        urunEkle(urunBilgileri)
    elif secim == 2:
        urunGuncelle(urunBilgileri)
    elif secim == 3:
        urunSil(urunBilgileri)
    elif secim == 4:
        listeGoruntuleme(urunBilgileri)
    elif secim == 5:
        print("Toplam Maliyet: " + str(toplamMaliyet(urunBilgileri)))
    elif secim == 6:
        print("Sistemden çıkış yapılıyor.")
        break
    else:
        print("Geçersiz bir seçim yaptınız...")
