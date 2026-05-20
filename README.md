# SecureCloud-K8s-DevSecOps

## Bitiruv Malakaviy Ishi (BMI)
**Mavzu:** Bulutli infratuzilmada xavfsiz va avtomatlashtirilgan konteyner orkestratsiyasi tizimini loyihalash va tadbiq etish (DevSecOps)

**Bajaruvchi:** Kompyuter injiniringi fakulteti 5-bosqich talabasi Sunnat Ermatov
**Ta'lim muassasasi:** Toshkent universitetining axborot texnologiyalari (TATU)

---

## Loyiha haqida umumiy ma'lumot
Ushbu loyihada an'anaviy ishlab chiqarish (production) muhitlaridagi dasturiy ta'minotni yetkazib berish zanjirini kiberhujumlardan himoya qilish, statik va dinamik tahlil tizimlarini avtomatlashtirish hamda Kubernetes klasteri xavfsizligini ta'minlash infratuzilmasi qurilgan. Loyihada namuna sifatida mikroxizmatlar arxitekturasidagi dastur olinib, uning atrofiga "Shift Left Security" prinsiplari asosida himoya qatlamlari loyihalashtirilgan.

## Infratuzilma tarkibi va vositalar:
1. **Terraform (IaC):** AWS bulutli provayderida Jenkins serveri va AWS EKS (Elastic Kubernetes Service) klasterini avtomatik va xavfsiz tarzda noldan qurish kodlari (`EKS-TF`, `Jenkins-Server-TF`).
2. **Jenkins (CI/CD):** Dastur kodini avtomatlashtirilgan pipeline orqali testlash, skanerlash va klasterga uzatish zanjiri (`Jenkins-Pipeline-Code`).
3. **SonarQube (SAST):** Manba kodining sifati va undagi xavfsizlik kamchiliklarini (vulnerabilities) dastlabki bosqichda aniqlash.
4. **Trivy (Container Security):** Docker obrazlarining ichidagi operatsion tizim va kutubxona zaifliklarini (CVE) chuqur skanerlash.
5. **Kubernetes (Orchestration):** Konteynerlarni deklarativ boshqarish va xavfsiz routingni ta'minlovchi manifest fayllari (`Manifest-file`).

## Loyihani ishga tushirish (Getting Started)
Loyihani lokal yoki bulutli muhitda ishga tushirish uchun ushbu omborni klon qiling:
```bash
git clone [https://github.com/ersuncoder/SecureCloud-K8s-DevSecOps.git](https://github.com/ersuncoder/SecureCloud-K8s-DevSecOps.git)