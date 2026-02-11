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
<img width="1105" height="702" alt="Screenshot 2026-02-11 at 23 03 49" src="https://github.com/user-attachments/assets/860bbe8c-779a-482d-ab15-3b6e599ac461" />


---


## 🚀 Hızlı Başlangıç

###  Postman ile Hemen Deneyin
Aşağıdaki butona basarak tüm koleksiyonu kendi Postman çalışma alanınıza tek tıkla aktarabilirsiniz:

[![Run in Postman](https://run.pstmn.io/button.svg)] ([<img src="https://run.pstmn.io/button.svg" alt="Run In Postman" style="width: 128px; height: 32px;">](https://app.getpostman.com/run-collection/27535489-ba7bd1e3-2fcd-408f-b6ae-e130b0d8fe75?action=collection%2Ffork&source=rip_markdown&collection-url=entityId%3D27535489-ba7bd1e3-2fcd-408f-b6ae-e130b0d8fe75%26entityType%3Dcollection%26workspaceId%3D53b71a5e-f292-4066-bceb-ed5e7f4e25a8#?env%5BReqRes%5D=W3sia2V5IjoiYmFzZVVybCIsInZhbHVlIjoiaHR0cHM6Ly9yZXFyZXMuaW4iLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6Imh0dHBzOi8vcmVxcmVzLmluIiwiY29tcGxldGVTZXNzaW9uVmFsdWUiOiJodHRwczovL3JlcXJlcy5pbiIsInNlc3Npb25JbmRleCI6MH0seyJrZXkiOiJhcGlfa2V5IiwidmFsdWUiOiJyZXFyZXNfZTRkMzhkOTY2ZDc5NGMzMGFiNGIwZDFlMmU3NWIwMDAiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoic2VjcmV0Iiwic2Vzc2lvblZhbHVlIjoicmVxcmVzX2U0ZDM4ZDk2NmQ3OTRjMzBhYjRiMGQxZTJlNzViMDAwIiwiY29tcGxldGVTZXNzaW9uVmFsdWUiOiJyZXFyZXNfZTRkMzhkOTY2ZDc5NGMzMGFiNGIwZDFlMmU3NWIwMDAiLCJzZXNzaW9uSW5kZXgiOjF9LHsia2V5IjoidXNlcklkIiwidmFsdWUiOiIiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IjEiLCJjb21wbGV0ZVNlc3Npb25WYWx1ZSI6MSwic2Vzc2lvbkluZGV4IjoyfSx7ImtleSI6InRva2VuIiwidmFsdWUiOiIiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiYW55Iiwic2Vzc2lvblZhbHVlIjoiUXB3TDV0a2U0UG5wamE3WDQiLCJjb21wbGV0ZVNlc3Npb25WYWx1ZSI6IlFwd0w1dGtlNFBucGphN1g0Iiwic2Vzc2lvbkluZGV4IjozfSx7ImtleSI6InRpbWUgbm93IiwidmFsdWUiOiIiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiYW55Iiwic2Vzc2lvblZhbHVlIjoiMDItMTEtMjAyNiAyMDoxMjowNiIsImNvbXBsZXRlU2Vzc2lvblZhbHVlIjoiMDItMTEtMjAyNiAyMDoxMjowNiIsInNlc3Npb25JbmRleCI6NH1d))



👨‍💻 **Geliştiren:** [Tarık Karabaş](https://github.com/trkkrbs)
