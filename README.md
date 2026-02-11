# 🚀 ReqRes API Automation Project

![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Newman](https://img.shields.io/badge/Newman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)

Bu proje, **ReqRes API** üzerinde uçtan uca test otomasyonu gerçekleştirmek amacıyla geliştirilmiştir. Testler **Postman** ile yazılmış, **Newman** ile koşturulmuş ve **GitHub Actions** ile CI/CD sürecine dahil edilmiştir.

---

## 🎯 Proje Kapsamı (Test Senaryoları)

Proje, gerçek bir kullanıcı akışını simüle eden aşağıdaki API uç noktalarını kapsar:

* 🔑 **Login:** Token çıkarımı yapılır.
* 👤 **Create User:** Yeni kullanıcı oluşturulur ve ID saklanır.
* 📋 **Get User List:** Kullanıcı listesi doğrulanır.
* 🔍 **Get Single User:** Belirli bir kullanıcı detayları kontrol edilir.
* 🔄 **Update User:** Kullanıcı bilgileri güncellenir.
* 🗑️ **Delete User:** Kullanıcı silme işlemi test edilir.

---

## 🛠️ Kullanılan Teknolojiler

| Araç | Açıklama |
| :--- | :--- |
| **Postman** | API isteklerinin oluşturulması ve test scriptlerinin yazımı. |
| **Newman** | Postman koleksiyonlarını terminal üzerinden çalıştırmak için. |
| **Newman HTML Extra** | Detaylı ve görsel test raporları üretmek için. |
| **GitHub Actions** | Otomatik test çalıştırma (CI) ve zamanlanmış (Cron) görevler. |
| **Node.js** | Çalışma ortamı. |

---

## 🚀 Yerel Çalıştırma (Local Run)

Projeyi kendi bilgisayarınızda çalıştırmak için:

1.  **Repoyu klonlayın:**
    ```bash
    git clone [https://github.com/trkkrbs/reqres-api-automation.git](https://github.com/trkkrbs/reqres-api-automation.git)
    ```
2.  **Bağımlılıkları yükleyin:**
    ```bash
    npm install
    ```
3.  **Testleri koşturun:**
    ```bash
    newman run collection.json -e environment.json -r htmlextra
    ```
    *Raporlar `reports` klasörü altında oluşturulacaktır.*

---

## ⚙️ CI/CD & GitHub Actions

Bu proje otomatik olarak test edilir:
- **Zamanlanmış (Cron):** Her Pazartesi otomatik çalışır.
- **Manuel:** GitHub üzerinden "Run workflow" butonu ile tetiklenebilir.

### Raporlara Nasıl Erişilir?
1. GitHub'da **Actions** sekmesine gidin.
2. En son başarılı olan **workflow run**'a tıklayın.
3. **Artifacts** bölümünden `newman-report` dosyasını indirin.

---

## 📊 Rapor Örneği
*(Buraya oluşturduğun HTML raporun bir ekran görüntüsünü eklersen çok daha profesyonel durur)*
`![Report Screenshot](./path-to-your-image.png)`

---
👨‍💻 **Geliştiren:** [Tarık Karabaş](https://github.com/trkkrbs)
