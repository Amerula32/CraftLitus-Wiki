# 📐 Parsel (Plot) Türleri & Satış

Kasaba arazileri parçalara ayrılabilir ve farklı işlevler için özelleştirilebilir.

---

## 🏡 Parsel (Plot) Türleri

Bulunduğunuz plot alanının türünü değiştirmek için `/plot set [tür]` komutunu kullanabilirsiniz:

| Plot Türü | Komut | Açıklama |
| :--- | :--- | :--- |
| **Default** | `/plot set reset` | Standart kasaba parselleri. |
| **Shop** | `/plot set shop` | Oyuncu marketleri ve dükkanlar için özel alan. |
| **Arena** | `/plot set arena` | Kasaba içinde PVP'nin serbest olduğu özel dövüş alanı. |
| **Embassy** | `/plot set embassy` | Başka kasaba veya ulus üyelerine kiralanabilen alan. |
| **Wilds** | `/plot set wilds` | Ağaç veya maden toplamak için kırma izni verilen alan. |

---

## 🛒 Parsel Satışı & Kiralama

Belediye Başkanı parsel satarak kasaba kasasına gelir sağlayabilir:

1. Satılacak parselin üzerine gelin ve komutu yazın:
   ```bash
   /plot fs <fiyat>
   ```
2. Bir üye parseli satın almak için parselin üzerine gelip şu komutu yazar:
   ```bash
   /plot claim
   ```
3. Parseli satıştan kaldırmak için:
   ```bash
   /plot nfs
   ```
