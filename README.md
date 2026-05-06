# Biznesingizni Keyingi Darajaga Ko'taring

## Fayl tavsifi
Bu loyiha `index.html` ichida to'liq **premium Business / Agency landing page** yaratadi. Sahifa quyidagi bo'limlarni o'z ichiga oladi:
- Navbar (Logo, Menu, Dark/Light toggle, Contact button)
- Hero Section
- Xizmatlarimiz / Services
- Bizning Afzalliklarimiz
- Portfolio / Ishlarimiz
- Nima uchun bizni tanlashadi?
- Mijozlarimiz Sharhlari
- Kontakt / Bog'lanish
- Footer

## Matnlarni o'zgartirish
`index.html` ichidagi matnlarni o'zingizga moslashtirish uchun kerakli bo'limlarni toping:
- Hero sarlavha va subtitle
- CTA tugmalar matni
- Xizmatlar va ularning tavsifi
- Afzalliklar, statistikalar va testimonial matnlar
- Kontakt ma'lumotlari

Har bir bo'lim yuqorida HTML kommentariy bilan belgilangan, masalan:
- `<!-- ================== HERO SECTION ================== -->`
- `<!-- ================== SERVICES SECTION ================== -->`
- `<!-- ================== ADVANTAGES SECTION ================== -->`
- `<!-- ================== PORTFOLIO SECTION ================== -->`
- `<!-- ================== CONTACT SECTION ================== -->`

## Rasmni almashtirish
`index.html` ichida rasmlar Unsplash-dan yuklangan. Har bir rasmdagi `src` attributini kerakli yangi Unsplash yoki Pexels havolasi bilan almashtiring.

Misol:
```html
<img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?auto=format&fit=crop&w=1100&q=80" alt="..." />
```

Agar siz mahalliy rasm ishlatmoqchi bo'lsangiz, `src`ga o'z fayl yo'lingizni yozing:
```html
<img src="assets/hero.jpg" alt="Hero rasm" />
```

## Ranglarni o'zgartirish
Tailwind rang sxemasi `index.html` ichida `tailwind.config` orqali o'rnatilgan:
- `brand-light` — #4f46e5
- `brand-dark` — #8b5cf6
- `brand-accent` — #22c55e
- `brand-soft` — #6366f1

Ushbu ranglarni o'zgartirish uchun `tailwind.config` bo'limidagi rang qiymatlarini yangilang.

Misol:
```js
colors: {
  brand: {
    light: '#4f46e5',
    dark: '#8b5cf6',
    accent: '#22c55e',
    soft: '#6366f1'
  }
}
```

## Dark/Light Mode
Sahifadagi `Dark/Light mode toggle` tugmasi LocalStorage yordamida holatni saqlaydi. Rang sxemasini yanada kuchaytirish uchun Tailwind `dark:` sinflaridan foydalaning.

## Faylni ishga tushirish
1. `d:\LandingPages\index.html` faylini brauzerda oching.
2. Agar lokal server ishlatishni xohlasangiz, har qanday oddiy HTTP serverdan foydalaning.

## Foydali eslatma
Agar sahifa juda og'ir yoki rasm o'lchamlari katta bo'lsa, rasm URLlariga `q=80` yoki `w=900` kabi parametrlarni qo'shish orqali yuklash tezligini oshiring.
