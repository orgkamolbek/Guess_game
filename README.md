# 🎲 Guess Game: Dynamic Number Match Engine

HTML5, CSS3 va Vanilla JavaScript asosida yaratilgan, foydalanuvchining mantiqiy fikrlash tezligini sinovchi interaktiv "Son topish" o'yini. Loyiha shartli tekshirish operatorlari, tasodifiy sonlar generatsiyasi hamda foydalanuvchi harakatiga qarab real vaqtda DOM elementlari va UI fonlarini dinamik o'zgartirish mexanizmini ko'rsatib beradi.

---

## 📝 Loyiha haqida

Dastur kompyuter tomonidan 1 dan 100 gacha bo'lgan oraliqda tasodifiy yashirilgan maxfiy sonni topishga asoslangan. Har bir kiritilgan noto'g'ri taxmindan so'ng, tizim foydalanuvchiga yo'nalish ko'rsatuvchi signallar beradi va sahifaning umumiy rangini o'zgartiradi. O'yinda urinishlar sonini hisoblovchi ichki taymer (Counter) hamda o'yin xotirasini yangilovchi tizim integratsiya qilingan.

---

## 📐 O'yin Logikasi va UI Holatlari (Decision-Making Workflow)

Kiritilgan son `Math.random()` orqali yaratilgan maxfiy raqam bilan taqqoslanganda, dastur quyidagi mantiqiy tarmoqlar bo'ylab harakatlanadi:

1. [ Bo'sh Qiymat ] ──► Agar maydon bo'sh bo'lsa, ogohlantirish beriladi va hisoblagich oshmaydi.
2. [ Guess > Target ] ──► Ko'rsatma: "Kichikroq son ayting... ⬇️" | Sahifa foni: Qizil (`#e74c3c`).
3. [ Guess < Target ] ──► Ko'rsatma: "Kattaroq son ayting... ⬆️" | Sahifa foni: Ko'k (`#3498db`).
4. [ Guess == Target ] ──► G'alaba! Sahifa foni: Yashil (`#2ecc71`) | `alert()` xabarnomasi chiqariladi.

---

## ⚡ Asosiy xususiyatlari (Features)

* 🔮 **Dynamic State Colors:** Har bir noto'g'ri yoki to'g'ri taxminga qarab brauzer fonining `transition: 0.5s` silliqlikda butunlay boshqa rang kiritish holatiga o'tishi.
* 🎲 **Secure Math Randomization:** `Math.floor(Math.random() * 100) + 1` formulasi orqali har safar mutlaqo yangi va takrorlanmas maxfiy son yaratish mexanizmi.
* 📊 **Live Attempt Counter:** Foydalanuvchining nechta inkremental urinish orqali g'alabaga erishganini hisoblab boruvchi dinamik ko'rsatkich.
* 🔄 **Soft State Reset:** Sahifani yangilamasdan (Reload qilmasdan), o'yin xotirasini, urinishlar hisoblagichini va kiritish maydonlarini tozalovchi `resetGame()` funksiyasi.
* 📦 **Glassmorphism Container:** UI dizaynda shaffof `rgba(255, 255, 255, 0.1)` konteyner elementidan foydalanilgan bo'lib, u zamonaviy va yengil vizual ko'rinish beradi.

---

## 🛠️ Texnologiyalar (Tech Stack)

* **HTML5** — Markazlashtirilgan interfeys shakli, son kiritish inputi va boshqaruv tugmalari.
* **CSS3 UI/UX** — Flexbox tizimi orqali ekranni vertikal va gorizontal tekislash, elementlarning `transform: scale(1.05)` hover effektlari.
* **Vanilla JavaScript (ES6+)** — JavaScript hodisalari (`onclick`), o'zgaruvchilar boshqaruvi va dinamik CSS manipulyatsiyasi (`document.body.style`).

---

## 🚀 Ishga tushirish (How to Run)

Loyiha hech qanday tashqi resurslarga va kutubxonalarga bog'liq bo'lmagan mustaqil arxitekturaga ega:

1. Repozitoriyni kompyuterga yuklab oling:
   ```bash
   git clone [https://github.com/orgkamolbek/guess-game.git](https://github.com/orgkamolbek/guess-game.git)
