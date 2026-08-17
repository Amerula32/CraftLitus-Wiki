# 💰 Ekonomi, Banka & Günlük Vergiler

Towny dünyasında düzenli bir ekonomi yürütmek vital öneme sahiptir.

---

## 🏦 Kasaba Bankası ve Parası

Kasabanın tüm claim ücretleri, vergi ödemeleri ve büyüme masrafları **Kasaba Bankası** üzerinden ödenir.

- Kasabaya para yatırma: `/t deposit <miktar>`
- Bakiye sorgulama: `/t` yazdığınızda çıkan `Bank:` kısmından takip edebilirsiniz.

---

## 💸 Günlük Vergi (Daily Upkeep) Mantığı

Her gece gerçek zamanlı olarak (Örn: **Saat 00:00**) sunucuda vergi saati gerçekleşir:

1. **Kasaba Vergisi:** Kasabanızın sahip olduğu claim sayısı arttıkça günlük sunucuya ödediği miktar artar.
2. **Yetersiz Bakiye:** Eğer kasaba bankanızda günlük vergiye yetecek kadar para yoksa, kasabanız **İflas (Bankrupt)** durumuna düşer ve 24 saat içinde ödeme yapılmazsa kasaba silinir!

---

## 📊 Üyelerden Vergi Toplama

Belediye Başkanı kasaba üyelerinden günlük veya sabit vergi toplayabilir:

```bash
/t set taxes <miktar>     # Her üyeden günlük alınacak vergi tutarı.
/t set plottax <miktar>   # Her parsel sahibinden alınacak parsel vergisi.
```
