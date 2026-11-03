# Texnik va mazmuniy review — Tuzatilgan nashr 1.1

**Tekshiruv sanasi:** 2026-11-03  
**Fayl:** `Ethical_Hackerlik_Sanati_320_Bet_TUZATILGAN_2026.pdf`  
**SHA-256:** `b47b5a6f0c5ca4fa5e85c81affba64b939e65d2058152264bab391e8d9bf2015`  
**Hajm:** 2,303,079 bayt  
**Sahifalar:** 320, A4, shifrlanmagan, matni ajratib olinadi.

## Nima yaxshi ishlagan?

- Tarkib 12 oy va 48 haftaga rejalashtirilgan; har bir haftada nazariya, xavf/himoya, mashq, natija va hisobot bloki bor.
- Lokal test-server, Nmap, tcpdump, ip route, hashing va sintetik loglarni tahlil qilish bo‘yicha bajariladigan misollar mavjud.
- PDF matnli (skanerlangan rasmlar to‘plami emas); manbalar qismi 307–308-sahifalarda bor.
- Xavfsizlik chegaralari va ruxsatni hujjatlashtirishga urg‘u berilgan.

## E’lon qilishdan oldingi asosiy muammolar

1. **Ko‘p takrorlanadigan shablon:** 48 haftaning ko‘pida ayni xavfsizlik cheklisti, “Bir xil ko‘rinadigan signal...” va `command not found`/`Permission denied` diagnostika satrlari deyarli so‘zma-so‘z takrorlanadi. Bu o‘quvchilarga qulay bo‘lishi mumkin, ammo texnik chuqurlik hisobiga sahifa hajmini kengaytiradi.
2. **Bo‘sh tahririy maydonlar:** 45 ta haftalik “Amaliy mashg‘ulot B” sahifasida `Expected` qiymati bo‘sh ko‘rinadi; masalan, 37 va 187-sahifalar. Bu to‘ldiriladigan ish daftari bo‘lsa, aniq belgilanishi kerak; aks holda kutilgan natija kiritilsin.
3. **Mavzuga mos kelmaydigan matn:** 111-sahifadagi “XSS va browser trust” mavzusining chuqur tahlili SQL/ORMga qaytadi. 135-sahifadagi “AD/LDAP va Kerberos” tahlilida Linux SUID/SGID haqida matn keltiriladi. Bu paragraflar alohida tekshirilsin.
4. **Tahririy qoldiqlar:** 15-sahifadagi `tenglas.` jumlasi tugallanmagan; 21-sahifada ikki nuqta (`emas..`), 19 va 43-sahifalarda jadval ichida izolyatsiyalangan `i`/`t` ko‘rinadi.
5. **Sahifa taqsimoti mazmun tengligi emas:** 160 sahifada nazariya va 160 sahifada amaliyot sarlavhasi mavjud, ammo bu haqiqiy vaqt, misollar sifati yoki qiyinchilik darajasida aniq 50/50 kafolatlamaydi.
6. **Muallif va litsenziya:** PDF metadata muallif sifatida shaxsni aniqlamaydi; ommaviy GitHub nashri uchun mualliflik, boshqa materiallardan foydalanish huquqi va aniq litsenziya siyosati belgilanmagan.
7. **Amaliy buyruqlarni QA:** Matnda ko‘plab buyruqlar bor, ammo bu audit ularni Kali/Windows/AD/cloud muhitida to‘liq bajarib tasdiqlamadi. Har bir hafta `expected/actual` log va test skriptlari bilan tekshirilsin.

## Tavsiya qilinadigan ustuvor tuzatishlar

| Ustuvorlik | Ish | Qabul mezoni |
| --- | --- | --- |
| P0 | Har bir hafta uchun aniq `Expected` va `Actual` qiymatlari yoki to‘ldirish talabi | Bo‘sh maydonlar ataylab qoldirilgani ravshan |
| P1 | 48 hafta bo‘yicha mavzuga aloqasiz paragraf va ortiqcha takrorlarni tahrir qilish | Har hafta kamida 1 noyob chuqur texnik tushuntirish va 1 mustaqil mashq |
| P1 | Buyruqlarni 2026-yilgi Kali va mos ruxsatli VMlar bilan smoke-test qilish | Natija, versiya va xatoliklar jadvali |
| P1 | Mualliflik/litsenziya va asl manba bog‘lanishlarini yakunlash | Publik README va PDF metadata mos |
| P2 | Texnik imlo, jadval kataklari va havolalar QA | Renderlar va to‘liq matn auditi PASS |

## Natija

**PDF strukturasi: PASS.**  
**Tuzilishi va o‘quv dasturi: mavjud.**  
**Professional nashr sifatida mazmuniy QA: hali PASS emas.**  
**Public Release: draft maqomi bilan chiqarish mumkin; final/verified nashr sifatida emas.**
