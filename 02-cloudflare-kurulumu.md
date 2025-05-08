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

1. [https://one.dash.cloudflare.com/](https://one.dash.cloudflare.com/) adresine gir  
2. Sol menuden **Zero Trust** sekmesine gel.
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




