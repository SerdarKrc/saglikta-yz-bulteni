# 🏥 Sağlık Teknolojileri Bülten Hazırlama & Arşiv Ekosistemi
> Health Tech Newsletter Automation Workspace

Bu depo (repository), küresel ve yerel sağlık teknolojileri, yapay zeka entegrasyonları, biyoteknoloji, dijital sağlık (digital health) ve medikal cihaz (MedTech) sektörlerindeki en güncel gelişmeleri derlemek, analiz etmek ve haftalık bültenler oluşturmak amacıyla yapılandırılmış bir **AI-destekli çalışma alanıdır**.

---

## 📁 Proje Yapısı

Proje, AI asistanının en yüksek doğrulukla ve yapılandırılmış kurallarla çalışabilmesi için optimize edilmiştir:

```
├── .gitignore                     # Git tarafından takip edilmeyecek geçici ve IDE dosyaları
├── bulten_talimati.md             # AI asistanı için bülten hazırlama kuralları ve şablonları
├── kaynak_veritabani.json         # Taranacak aktif akademik, sektörel ve haber kaynaklarının veri tabanı
└── arsiv/                         # Üretilen haftalık bültenlerin saklandığı arşiv klasörü
    ├── README.md                  # Arşiv klasörü isimlendirme kuralları ve açıklaması
    └── bulten_2026-05-27.md       # 27 Mayıs 2026 tarihli bülten çıktısı (örnek)
```

---

## 🚀 Başka Bir Bilgisayarda Nasıl Çalıştırılır?

Bu çalışma alanı, **AI Asistanı Entegrasyonlu Editörler** (VS Code + Gemini/Claude/Copilot veya Cursor) ile çalışacak şekilde tasarlanmıştır. Projeyi başka bir bilgisayara taşıyıp çalıştırmak için:

### 1. Dosyaları Yeni Bilgisayara Aktarın
Bu depoyu GitHub'a yükledikten sonra, diğer bilgisayarınızda bir terminal açıp projeyi klonlayabilirsiniz:
```bash
git clone <github-depo-linkiniz>
```
*(Alternatif olarak projeyi ZIP olarak indirip diğer bilgisayara açabilirsiniz.)*

### 2. Klasörü IDE (Editör) ile Açın
Klonladığınız veya ayıkladığınız `IDE Sağlıkta Yapay Zeka` klasörünü **VS Code** veya **Cursor** gibi bir kod editörüyle açın.

### 3. AI Asistanına Talimat Verin
Editörünüzdeki yapay zeka asistanına (Gemini, Claude vb.) şu şekilde seslenin:

> *"Lütfen [bulten_talimati.md](file:///bulten_talimati.md) dosyasındaki kuralları ve [kaynak_veritabani.json](file:///kaynak_veritabani.json) içindeki aktif kaynakları kullanarak bu haftanın Sağlık Teknolojileri Bültenini hazırla. Sonuçları `arsiv/bulten_YYYY-AA-GG.md` formatında kaydet."*

Yapay zeka asistanı web araması yaparak güncel haberleri toplayacak, çevirecek, özetleyecek ve bülteni belirtilen şablona göre otomatik olarak oluşturacaktır.

---

## 💻 GitHub'a Yükleme Rehberi (Nasıl Paylaşılır?)

Bu projeyi ilk kez GitHub'a yüklemek için aşağıdaki adımları takip edebilirsiniz:

### Yöntem A: Git Komut Satırı (CLI) ile Yükleme
Bilgisayarınızda Git yüklüyse, proje dizininde şu komutları sırasıyla çalıştırın:

1. **Git deposunu başlatın:**
   ```bash
   git init
   ```
2. **Tüm dosyaları hazırlık alanına ekleyin:**
   ```bash
   git add .
   ```
3. **İlk commit'i yapın:**
   ```bash
   git commit -m "Initial commit: Bülten şablonları ve kaynak veritabanı"
   ```
4. **Ana dalı belirleyin:**
   ```bash
   git branch -M main
   ```
5. **GitHub'da yeni bir boş depo oluşturun** ve onun bağlantısını projeye ekleyin:
   ```bash
   git remote add origin https://github.com/KULLANICI_ADINIZ/DEPO_ADINIZ.git
   ```
6. **Dosyaları GitHub'a gönderin:**
   ```bash
   git push -u origin main
   ```

### Yöntem B: GitHub Desktop Kullanarak (Kodsuz)
1. [GitHub Desktop](https://desktop.github.com/) uygulamasını indirin ve kurun.
2. **File > Add Local Repository** seçeneğine tıklayın.
3. Bu klasörü (`IDE Sağlıkta Yapay Zeka`) seçin.
4. Uygulama size *"Bu klasör bir git deposu değil, oluşturmak ister misiniz?"* diyecektir. **Create a Repository** seçeneğine tıklayarak oluşturun.
5. Değişiklikleri açıklayıp **Commit** butonuna basın.
6. Sağ üstteki **Publish Repository** butonuna tıklayarak doğrudan GitHub hesabınıza yükleyin.
