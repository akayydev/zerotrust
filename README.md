<h1 align="center">🛡️ Zero Trust ile Discord Erişim Engeli Aşma Rehberi</h1>

<p align="center">
  <i>Discord'un kısıtlandığı bölgelerde (ülke engeli, IP banı vs.) <b>Zero Trust Network Access (ZTNA)</b> ile erişimi geri kazan!</i><br>
  <sub>örnek: Türkiye gibi 🙈</sub>
</p>

---

## 🎯 Amaç

- IP engelleri, port bloklamaları ve DNS sorunlarını aşmak  
- Tüm trafiği güvenli, şifreli ve kontrollü biçimde yönlendirmek  
- VPN olmadan kendi tünel altyapını kurmak  
- Chrome üzerinden Discord erişimini kalıcı hale getirmek  

---

## 🧰 Kullanılan Yöntemler

- 🔐 Zero Trust Proxy Kurulumu ( Cloudflare Tunnel / WARP )  
- 🔄 mTLS (karşılıklı TLS) ile şifreli bağlantı  
- 🚧 Discord IP’lerinin Whitelist ve Bypass ayarları    
  
---

## 📂 Rehber Dosyaları - Kurulum Aşamaları

- [`01-zero-trust-nedir.md`](01-zero-trust-nedir.md) – Basit kavramlar  
- [`02-cloudflare-kurulumu.md`](02-cloudflare-kurulumu.md) – Cloudflare + WARP ile tünel oluşturma 
- [`03-ip-ve-dns.md`](03-ip-ve-dns.md) – IP adresleri ve Domain'ler

---

## ⚠️ Uyarı

Bu içerik tamamen **eğitim ve kişisel erişim** amaçlı hazırlanmıştır.  
Ticari, yasa dışı veya kötüye kullanım durumları yasal sorumluluk doğurabilir.

---

IP adreslerini bazı durumlarda güncelliyorum şuan ki IP'ler fazlası ile yeterlidir.

---

<p align="center">
  <b>Hazırlayan:</b> <a href="https://github.com/ardakay19">Akay</a> <br>
</p>
