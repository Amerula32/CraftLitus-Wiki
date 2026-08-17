# 🔐 İzinler ve Güvenlik Yönetimi

Kasabanızdaki blok kırma, koyma, sandık açma veya şalter kullanma gibi eylemleri kimlerin yapabileceğini ayrıntılı olarak özelleştirebilirsiniz.

---

## 👥 İzin Grupları

Towny sisteminde 4 ana grup bulunur:

1. **Resident (Sakinler):** Kasabanıza kayıtlı olan üyeler.
2. **Nation (Ulus):** Ulusunuzdaki diğer kasabaların üyeleri.
3. **Ally (Müttefikler):** Müttefik ulus ve kasaba üyeleri.
4. **Outsider (Yabancılar):** Kasabanızda veya ulusunuzda olmayan tüm diğer oyuncular.

---

## ⚙️ İzin Ayarlama Komutu Syntax'ı

```bash
/t set perm [Grup] [Eylem] [on/off]
```

### Eylem Türleri:
- `build`: Blok koyma izni.
- `destroy`: Blok kırma izni.
- `switch`: Şalter, kapı, düğme kullanma izni.
- `itemuse`: Kovayla su/lava alma, eşya çerçevesi kullanma izni.

---

## 📝 Örnek Kullanımlar

{% hint style="danger" %}
**Dikkat:** Yabancılara (`outsider`) asla `build` veya `destroy` izni vermeyin! Aksi takdirde kasabanız yağmalanabilir.
{% endhint %}

```bash
# Yabancıların düğme ve kapı kullanmasını engelle:
/t set perm outsider switch off

# Kasaba sakinlerinin blok koyup kırmasına izin ver:
/t set perm resident build on
/t set perm resident destroy on

# Tüm kasaba izinlerini sıfırla:
/t set perm reset
```
