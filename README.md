# 🎨 Biznes Studio — Premium Landing Page Shabloni

Bu **Soff.uz uchun maxsus tayyorlangan**, zamonaviy va yuqori konversiyali Business / Agency landing page. Kod toza, kommentariylar batafsil va o'zingizga moslashtirish osondir.

---

## 📋 Mundarija
1. [Nima bu?](#nima-bu)
2. [Fayllar strukturasi](#fayllar-strukturasi)
3. [Asosiy o'zgartirishlari](#asosiy-ozgartirishlari)
4. [O'zbekcha Kommentariylar](#ozbekcha-kommentariylar)
5. [Ranglar va Dinamika](#ranglar-va-dinamika)
6. [Brauzer va Mobil Qo'llab-Quvvatlash](#brauzer-va-mobil-qollab-quvvatlash)
7. [Tez Maslahatlar](#tez-maslahatlar)

---

## 🎯 Nima bu?

**Biznes Studio** — premium, modernistik va responsive landing page. Quyidagi xususiyatlari mavjud:

✅ **Scroll animatsiyalar** — elementlar chapdan, o'ngdan, yuqoridan kiradi  
✅ **Portfolio hover effektlari** — rasmlar ustida ma'lumot ko'rinadi  
✅ **Dark/Light rejim** — foydalanuvchi tanlab oladi  
✅ **Mobil-dost** — barcha ekranlarda mukammal ko'rinadi  
✅ **Tez yuklash** — Tailwind CSS va vanilla JavaScript  
✅ **SEO-optimized** — meta teglar va semantik HTML  

---

## 📁 Fayllar Strukturasi

```
d:\LandingPages\
├── index.html          ← Asosiy landing page (bu faylni o'zgartirasiz)
└── README.md           ← Bu dokumentatsiya
```

Hozircha faqat **index.html** va **README.md** bor. Agar CSS yoki JS alohida fayllar kerak bo'lsa, ularni qo'shishingiz mumkin.

---

## 🔧 Asosiy O'zgartirishlari (Eng Muhim Joylar)

### 1️⃣ Kompaniya Nomini O'zgartirish

**Noma'lumida izohni qidiring:** "Bu yerga kompaniya nomi yoziladi"

Quyidagi joylardan o'zgartirish kerak:

```html
<!-- NAVBAR'da -->
<p class="text-sm font-semibold">Biznes Studio</p>
<p class="text-[11px] text-slate-400">Premium Agency</p>

<!-- FOOTER'da -->
<p class="text-lg font-semibold text-slate-950 dark:text-white">Biznes Studio</p>
```

**Masalan:** "Biznes Studio" o'rniga "Digital Solutions" yozing.

---

### 2️⃣ Hero Section (Eng Katta Sarlavha)

**Qidiring:** "Bu yerga katta va ta'sirli sarlavha yozing"

```html
<h1 class="scroll-reveal text-5xl font-extrabold...">
  <span class="block">Biznesingizni</span>
  <span class="block bg-gradient-to-r from-brand-light via-brand-dark to-brand-accent...">
    premium hamkorlik
  </span>
  <span class="block">bilan onlayn maydonda kuchaytiring.</span>
</h1>
```

**O'zgartirishlari:**
- Har bir `<span>` — yangi qatorga o'tadi
- Rangni o'zgartirish uchun `bg-gradient-to-r from-brand-light...` kismini tahrirlang
- Shuning asosida — `<p>` tagida tavsif matni bor

---

### 3️⃣ Lead Matn (Kichik Tavsif)

**Qidiring:** "Bu yerga qisqa va aniq lead matn kiriting"

```html
<p class="scroll-reveal max-w-xl text-lg leading-8 text-slate-600...">
  Soff.uz platformasi uchun maxsus ishlab chiqilgan, zamonaviy va yuqori 
  konversiyali biznes landing page...
</p>
```

Bu — sarlavhaning ostidagi qisqa, persuasiv matn.

---

### 4️⃣ CTA Tugmalari (Chaqiriqlar)

**Qidiring:** "Bugun boshlash" yoki "Xizmatlarimiz"

```html
<a href="#contact" class="inline-flex ... bg-brand-accent ...">
  Bugun boshlash
</a>
<a href="#services" class="inline-flex ... border border-slate-200 ...">
  Xizmatlarimiz
</a>
```

**O'zgartirish:**
- Matn: `Bugun boshlash` o'rniga boshqasi yozing
- Rang: `bg-brand-accent` = yashil; `border border-slate-200` = oq

---

### 5️⃣ Xizmatlar (Services Section)

**Qidiring:** "Xizmatlarimiz" yoki `id="services"`

```html
<article class="reveal-left group...">
  <div class="mb-6 inline-flex h-16 w-16 ... bg-brand-light/10 ...">💡</div>
  <h3 class="text-xl font-semibold...">Brend Strategiyasi</h3>
  <p class="mt-3 text-slate-500...">Har bir brend uchun noyob...</p>
</article>
```

**O'zgartirishlari:**
- **Emoji:** `💡` o'rniga boshqasini qo'ying
- **Sarlavha:** "Brend Strategiyasi" → O'zingizning xizmatini yozing
- **Tavsif:** `<p>` tagida yangi tavsif yozing
- **Rang:** `bg-brand-light/10` o'rniga `bg-brand-dark/10` yoki boshqa variant

---

### 6️⃣ Portfolio (Ishlar Namunasi)

**Qidiring:** `id="portfolio"`

```html
<article class="group relative overflow-hidden...">
  <img src="https://images.unsplash.com/photo-1519337265831..." 
       alt="Agentlik veb-sayt dizayni" 
       class="h-72 w-full object-cover..." />
  <div class="absolute inset-x-0 bottom-0 p-6 ... opacity-0 group-hover:opacity-100">
    <p class="text-xs uppercase ... text-brand-accent">Raqamli kampaniya</p>
    <h3 class="mt-3 text-2xl font-semibold">Innovatsion landing page</h3>
    <p class="mt-3 text-sm text-slate-200">Ajratilgan brend maydoni...</p>
  </div>
</article>
```

**O'zgartirishlari:**
- **Rasm URL'si:** `src="https://images.unsplash.com/photo-..."` ni o'zingizning rasming URL'iga almashtiring
- **Alt tekst:** `alt="Agentlik veb-sayt dizayni"` — SEO uchun muhim
- **Kategoriya:** `<p>` ga "Raqamli kampaniya" o'rniga turini yozing
- **Sarlavha va tavsif:** Hover'da ko'rinadigan matn

---

### 7️⃣ Kontakt Bo'limi (Contact Section)

**Qidiring:** `id="contact"`

```html
<div class="rounded-[2rem] bg-white p-8 text-center ...">
  <p class="text-sm uppercase ... text-slate-500">Telegram</p>
  <a href="https://t.me/YOUR_TELEGRAM" target="_blank" ...>
    @YOUR_TELEGRAM
  </a>
  <p class="mt-3 text-sm text-slate-500 ...">Tez va shaxsiy maslahat uchun.</p>
</div>
```

**O'zgartirishlari:**
- **Telegram:** `https://t.me/YOUR_TELEGRAM` → O'zingizning Telegram username'ini yozing (masalan: `https://t.me/myagency`)
- **Telefon:** `tel:+998901234567` → O'zingizning raqamini yozing
- **Email:** `mailto:hello@biznesstudio.uz` → O'zingizning emailini yozing

---

## 💬 O'zbekcha Kommentariylar

Koddagi **har bir muhim joy** o'zbekcha kommentariyga ega:

```html
<!-- Bu yerga logotip yoki brend qisqartmasi yoziladi -->
<span>B</span>

<!-- Bu yerga kompaniya nomi yoziladi -->
<p class="text-sm font-semibold">Biznes Studio</p>

<!-- Bu yerga katta va ta'sirli sarlavha yozing -->
<h1 class="scroll-reveal ...">Biznesingizni...</h1>

<!-- Bu yerga qisqa va aniq lead matn kiriting -->
<p class="scroll-reveal ...">Soff.uz platformasi uchun...</p>
```

**Kommentariylar shunis bildiradi:**
- "Bu yerga" → oxolingiz o'zgartirasiz
- "Bu yerga O'Z" → faqat siz kiritasiz
- "O'zgartirish uchun" → avval bosh bilan o'ylab olasiz

---

## 🎨 Ranglar va Dinamika

### Asosiy Ranglar

```javascript
brand: {
  light: '#4f46e5',      // Indigo (asosiy rang)
  dark: '#8b5cf6',       // Violet (ko'p ishlatiladigan)
  accent: '#22c55e',     // Yashil (CTA tugmalari)
  soft: '#6366f1'        // Yumshoq indigo
}
```

**O'zgartirish uchun:**
- `style` tagida yoki tailwind classesida rang nomi bor
- Masalan: `text-brand-light` → "Bu element indigo rang bilan"
- `bg-brand-accent` → "Bu fon yashil"

### Animatsiyalar

```css
.scroll-reveal {
  opacity: 0;
  transform: translateY(32px);
  transition: opacity 0.9s ease, transform 0.9s ease;
}

.scroll-reveal.active {
  opacity: 1;
  transform: translateY(0);
}
```

- **reveal-left** — chapdan kiradi
- **reveal-right** — o'ngdan kiradi
- **scroll-reveal** — yuqoridan kiradi

JavaScript bu elementlarni kuzatadi va scroll vaqtida "active" classini qo'shadi.

---

## 🌐 Brauzer va Mobil Qo'llab-Quvvatlash

**Bu landing page quyidagida ishlaydi:**

✅ Chrome, Firefox, Safari, Edge (hammasida)  
✅ iPhone, Android, iPad (barcha mobillar)  
✅ Desktoplarda (wide screens)  

**Responsive breakpoints:**
- `sm:` — 640px+ (kichik mobillar)
- `md:` — 768px+ (planshetlar)
- `lg:` — 1024px+ (desktoplar)
- `xl:` — 1280px+ (katta monitorlar)

Misol:
```html
<div class="p-4 md:p-8 lg:p-12">
  <!-- 4px mobilhda, 8px planshetda, 12px desktopda -->
</div>
```

---

## ⚡ Tez Maslahatlar

### 1. Saytni Ko'rish
1. VS Code'da **index.html** ni oching
2. O'ng klik → "Open with Live Server" (agar Extension o'rnatilgan bo'lsa)
3. Yoki fayl nomi'ga o'ng klik → "Open in default browser"

### 2. Dark Rejimni Test Qilish
- Saytning o'ng ust burchagida ☀️ tugmasi bor
- Bosing → Dark/Light almashadi
- Browser localStorage'da saqlanadi

### 3. Mobil Ko'rinishni Test Qilish
- Chrome DevTools: F12
- Ctrl + Shift + M (yoki hamburger → "Toggle device toolbar")
- Mobil ekranda qaytib ko'rin

### 4. SEO Tavsifi
- `<title>` → Qidiruv natijasida ko'rinadi
- `alt="..."` → Rasm tavsifi (SEO muhim)
- Sarlavhalar (`<h1>`, `<h2>`) → Struktura uchun

### 5. Performance
- Tailwind CSS inline → tez yuklash
- Unsplash rasmlar (cache bilan) → optimal
- Vanilla JS → hafif va tez

---

## 📝 O'zgartirishlari Qo'plab Qilish (Agar Yangi Fayllar Kerak Bo'lsa)

Agar CSS yoki JS alohida qilishni xohlasangiz:

```
index.html (asosiy)
├── styles.css (custom CSS)
└── script.js (custom JS)
```

Lekin hozir hamma **inline** — bir faylda.

---

## ✨ Yakuniy Maslahatlar

1. **Rasmlarni Sifatli Qiling** — Unsplash, Pexels, Pixabay'dan olasiz
2. **Matnni Qisqa Qiling** — Oqilona va haybat bo'lsin
3. **Rang Palitrasini Aniqlang** — Ko'p rang bo'lmasin
4. **Mobile First** — Mobilhda test qilib, keyin desktop
5. **A/B Testing** — CTA tugmasini sinovdan o'tkazasiz
6. **Google Analytics** — Sizning trafiking nechcha?

---

## 🎓 Qo'shimcha Resurslar

- **Tailwind CSS** — https://tailwindcss.com
- **Unsplash Rasmlar** — https://unsplash.com
- **Color Picker** — https://htmlcolorcodes.com
- **Font Awesome** — https://fontawesome.com

---

## 📞 Savol-Javob

**S:** Rasmlarni qanday o'zgartiraman?  
**J:** `src="https://..."` URL'ini o'zingizning rasming URL'iga almashtiring.

**S:** Rangni qanday o'zgartiram?  
**J:** `brand-light`, `brand-dark` va boshqalarni hex kodiga (`#FF0000`) almashtiring.

**S:** Mobilhda nima qiladim?  
**J:** `sm:`, `md:`, `lg:` prefixli classlar mavjud — ular automatic o'zgaradi.

**S:** Animatsiyalarni o'chirishlari mumkin bo'lasimi?  
**J:** CSS'da `transition: none;` qo'shasiz.

---

**✅ Tayyor! Endi o'zingizga moslab ishlatasiz.**
