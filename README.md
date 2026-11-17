# 🟢 Ozod — qarzlardan ozod boʻling

**Ozod** — oʻzbek tilidagi shaxsiy buxgalter ilovasi. Qarzlaringiz, oylik daromad va xarajatlaringizni kiritasiz — ilova hisoblaydi, tahlil qiladi, toʻlov kunlarini eslatadi va qarzdan eng tez qutulish rejasini tuzib beradi.

## Imkoniyatlar

- 💳 **Qarzlar** — bank krediti yoki shaxsdan olingan qarz, foiz, oylik toʻlov, toʻlov kuni, toʻlovlar tarixi
- ➕➖ **Kirim-chiqim** — toifalar boʻyicha daromad va xarajatlar, har oy takrorlanadigan yozuvlar (maosh, ijara…)
- 📊 **Tahlil** — oylik hisobot, 6 oylik grafik, xarajat toifalari
- 🎯 **Qutulish rejasi** — “Koʻchki” (eng yuqori foiz birinchi) va “Qor koʻpchigi” (eng kichik qarz birinchi) strategiyalari, qarzdan ozod boʻlish sanasi, tejaladigan foiz
- ⏰ **Eslatmalar** — ilovada ogohlantirish, brauzer bildirishnomasi va telefon kalendariga (.ics) har oylik eslatma
- ✨ **AI maslahatchi** — oflayn tahlil + Google Gemini orqali savol-javob (bepul API kalit bilan)
- 💾 **Zaxira** — maʼlumotlarni JSON faylga saqlash va tiklash
- 📱 **Telefonga oʻrnatiladi** (PWA), internetsiz ham ishlaydi

Barcha maʼlumotlar faqat sizning qurilmangizda saqlanadi.

## GitHub Pages orqali ishga tushirish

1. GitHub’da yangi repozitoriy yarating (masalan `ozod`), **Public** qilib.
2. **Add file → Upload files** orqali shu papkadagi barcha fayllarni yuklang: `index.html`, `manifest.json`, `sw.js`, `icon.svg`, `README.md`.
3. **Settings → Pages** boʻlimida *Source*: `Deploy from a branch`, *Branch*: `main` / `(root)` → **Save**.
4. 1–2 daqiqadan keyin ilova shu manzilda ochiladi: `https://SIZNING-LOGIN.github.io/ozod/`
5. Telefonda oching → brauzer menyusidan **“Bosh ekranga qoʻshish”** (Android: *Install app*, iPhone Safari: *Share → Add to Home Screen*).

## AI ni ulash

1. https://aistudio.google.com saytiga kiring → **Get API key** → kalit yarating.
2. Ozod → ⚙️ Sozlamalar → *Gemini API kaliti* ga joylang → Saqlash.
3. Model nomi standart: `gemini-2.5-flash` (kerak boʻlsa oʻzgartirish mumkin).

## Texnologiya

Bitta `index.html` fayl — toza HTML/CSS/JavaScript, hech qanday kutubxona yoki server kerak emas. Maʼlumotlar `localStorage` da saqlanadi.
