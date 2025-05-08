# 🌐 Cloudflare Tunnel ile Zero Trust Kurulumu

Bu bölümde, Cloudflare üzerinden bir **Zero Trust Tüneli** kurarak Discord trafiğini güvenli şekilde yönlendirmeyi öğreneceğiz. Bu yapı sayesinde IP engelleri ve DNS sınırlamaları kolayca aşılabilir. 
## 📌 Bu yapı Discord dışında diğer engelli servislerde de çalışabilir

---

## 🔧 GEREKSİNİMLER

- Bir adet Cloudflare hesabı yoksa bu linkten oluşturunuz. ([https://dash.cloudflare.com](https://dash.cloudflare.com))
- Windows / Linux yüklü bir cihaz
- WARP uygulaması ([https://one.one.one.one/](https://one.one.one.one/))

---

## 🧱 1. Cloudflare Zero Trust Panelini Aç

1. Cloudflare hesabınızı oluşturduktan sonra; [https://one.dash.cloudflare.com/](https://one.dash.cloudflare.com/) adresine girin. 
2. Sol menuden **Zero Trust** sekmesine gelin.
3. Takımın adını oluşturun. (Giriş yaparken bu ad lazım olucak sallamayın.)
4. Free paketini seçip **Select plans** diyoruz.
5. Kart bilgilerimizi yazıp ilerliyoruz. **Karttan para çekmeyecektir ücretsiz sürümü kullannıyor doğrulama amaçlı kart bilgisi ister.**
6. Team kurulumu tamamlandıktan sonra seni Zero Trust paneline yönlendirecek. Artık Tunnel oluşturma aşamasına geçebiliriz!

---

## 2. Zero Trust Kurulumu

Sol sekmeden **Access > Policies** kısmına gelin. **Add a Policy** seçeneğini seçin.

![image](https://github.com/user-attachments/assets/637e8de9-ebf2-47f4-85bf-e641a3086d2e)
![image](https://github.com/user-attachments/assets/b3ea4302-f154-4b53-8942-8c954b63f4f1)

Ayarlarınızı bu şekilde yaptıktan sonra aşağı kaydırıp kaydedin.
Yaptıklarınızın aynısını **Access > Rule Groups** seçeneği içinde yapıp kaydedin.


## Discord'u tünellemek

 Sol sekmeden **Settings > Warp Client** sekmesini açın.
 **Device enrollment permissions** seçeneğinin yanındaki **Manage** sekmesine basın.
 
![image](https://github.com/user-attachments/assets/a4566020-77ac-4d1b-87a3-9d2d8cfff7a3)

Oluşturduğunuz **Policies'i** burada seçiniz.
Save edip **Back to Settings** seçeneği ile geri dönün.
**Device settings > Profile settings >> Configure** seçeneğine basın.

![image](https://github.com/user-attachments/assets/e0cb8a9a-1ff5-4475-aa15-fb7fc27936b8)

En aşağı kaydırıp **Split Tunnels** seçeneğini **Exclude IPs and domains >> Include IPs and domains** seçeneğine çevirip onaylayın.

![image](https://github.com/user-attachments/assets/eeaa22dd-da94-467d-975a-64dcb1bafb99)

**Manage** seçeneğine basıp [`03-ip-ve-dns.md`](03-ip-ve-dns.md) bu kısımdaki tüm domain ve ip adreslerini tek tek yapıştırıyoruz. Description seçeneğini boş bırakabilirsiniz.

**Back to Profile** seçeneğine basıp geri döndükten sonra **Device tunnel protocol** ayarını resimdeki MASQUE protocolune çeviriyoruz.
![image](https://github.com/user-attachments/assets/8992a376-2617-4d25-9cc5-b7a95ec35245)

En aşağıya kaydırıp kaydettikten sonra Chrome üzerinden ayarlamalarımız tamam.


Daha sonra başta indirdiğimiz WARP uygulamasını kuruyoruz.
![image](https://github.com/user-attachments/assets/f52fa3cb-1d52-4850-8fe7-fb715b4c9d6e)

Sağ alttan **Ayarlar > Tercihler > Hesap ve _Cloudflare Zero Trust ile oturum aç_** seçeneğine basıyoruz. 
Açılan yeni sekmede ileri basıp, çıkan sekmeyi kabul et diyip ilerliyoruz.

![image](https://github.com/user-attachments/assets/458ad7f2-b491-445a-adff-57f47f824f2d)

Bu sekmeye ulaştığınız zaman en başta oluşturmuş olduğunuz takım adını yazıp yönlendirilen **Warp Login App** sayfasında aktif olarak kullandığınız bir email girip postanıza gelen kodu yazdıktan sonra giriş yapmış oluyorsunuz.

![image](https://github.com/user-attachments/assets/df115519-3d77-44f0-8237-eccb64375df6)

Bu sayfayı gördüyseniz başarılı bir şekilde Discordu tünellemişsinizdir. Eğer IP ve DOMAIN'leri eksiksiz girdiyseniz Chrome üzerinden de Discord erişimi açılmış olacaktır.









