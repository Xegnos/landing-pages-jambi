# Image Replacement Guide

This guide shows you exactly where to add images in each template.

---

## GYM TEMPLATE (gym.html)

### 1. Hero Section Background
**Line to find:** Search for `.hero-image-placeholder`

```css
/* BEFORE */
.hero-image-placeholder {
    background: linear-gradient(135deg, var(--black-lighter) 0%, var(--black) 100%);
}

/* AFTER */
.hero-image-placeholder {
    background: url('images/gym/hero.jpg') center/cover no-repeat;
}
```

**Recommended image:** Action shot of gym interior or someone working out (1920x1080px)

---

### 2. Coach Photos
**Line to find:** Search for `.coach-image-placeholder`

**Option A: Keep as background (easier)**
Add this CSS for each coach:
```css
.coach-card:nth-child(1) .coach-image {
    background: url('images/gym/coach-reza.jpg') center/cover no-repeat;
}
.coach-card:nth-child(2) .coach-image {
    background: url('images/gym/coach-diana.jpg') center/cover no-repeat;
}
.coach-card:nth-child(3) .coach-image {
    background: url('images/gym/coach-andi.jpg') center/cover no-repeat;
}
.coach-card:nth-child(4) .coach-image {
    background: url('images/gym/coach-maya.jpg') center/cover no-repeat;
}
```

**Option B: Use img tags (better for SEO)**
Find in HTML:
```html
<div class="coach-image">
    <div class="coach-image-placeholder">
        <svg><use href="#icon-user"/></svg>
    </div>
    <span class="coach-specialty">Strength & Conditioning</span>
</div>
```

Replace with:
```html
<div class="coach-image">
    <img src="images/gym/coach-reza.jpg" alt="Coach Reza Pratama">
    <span class="coach-specialty">Strength & Conditioning</span>
</div>
```

Add this CSS:
```css
.coach-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center top; /* focuses on face */
}
```

**Recommended image:** Professional headshot or action pose (500x600px)

---

### 3. Facility Images (Optional)
If you want images for each facility card:

```css
.facility-card:nth-child(1) {
    background: linear-gradient(rgba(0,0,0,0.8), rgba(0,0,0,0.9)), url('images/gym/weight-area.jpg') center/cover;
}
.facility-card:nth-child(2) {
    background: linear-gradient(rgba(0,0,0,0.8), rgba(0,0,0,0.9)), url('images/gym/cardio-zone.jpg') center/cover;
}
/* ... repeat for other facilities */
```

---

## SPA TEMPLATE (spa.html)

### 1. Hero Section
Search for `.hero-visual` or gradient backgrounds in hero

```css
/* Add background to hero section */
.hero {
    background: linear-gradient(rgba(0,0,0,0.3), rgba(0,0,0,0.5)), url('images/spa/hero.jpg') center/cover no-repeat;
}
```

### 2. Service Cards
Find `.service-image-placeholder` or similar:

```css
.service-card:nth-child(1) .service-image {
    background: url('images/spa/volcanic-stone.jpg') center/cover;
}
.service-card:nth-child(2) .service-image {
    background: url('images/spa/aromatherapy.jpg') center/cover;
}
/* ... etc */
```

---

## WEDDING TEMPLATE (wedding.html)

### 1. Hero Grid Images
Find the hero image grid in HTML:

```html
<div class="hero-image">
    <div class="hero-image-placeholder">Pre-wedding<br>Session</div>
</div>
```

Replace with:
```html
<div class="hero-image">
    <img src="images/wedding/prewedding.jpg" alt="Pre-wedding Session">
</div>
```

Add CSS:
```css
.hero-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}
```

### 2. Portfolio Gallery
Find portfolio items and replace:

```html
<div class="portfolio-item">
    <img src="images/wedding/portfolio-1.jpg" alt="Andi & Sari Wedding">
    <div class="portfolio-overlay"><span>Lihat Cerita</span></div>
</div>
```

---

## KOREAN BBQ TEMPLATE (kbbq.html)

### 1. Menu Card Images
Find `.menu-card-image`:

```css
.menu-card:nth-child(1) .menu-card-image {
    background: url('images/kbbq/paket-reguler.jpg') center/cover;
}
.menu-card:nth-child(2) .menu-card-image {
    background: url('images/kbbq/paket-premium.jpg') center/cover;
}
```

### 2. Meat Cuts Section
For individual meat images:

```css
.cut-card:nth-child(1) {
    background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.8)), url('images/kbbq/beef-slice.jpg') center/cover;
}
```

---

## NOTARIS TEMPLATE (notaris.html)

### 1. Profile Photo
Find the about section with lawyer profile:

```css
.about-image {
    background: url('images/notaris/dharma-wijaya.jpg') center/cover;
}
```

### 2. Office Photo
```css
.hero-bg {
    background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.8)), url('images/notaris/office.jpg') center/cover;
}
```

---

## QUICK CHECKLIST

For each template, you typically need:

- [ ] 1 Hero/banner image (1920x1080)
- [ ] 4-6 Service/product images (600x400)
- [ ] 3-4 Team/staff photos (500x600)
- [ ] 1 Logo (200x200, PNG transparent)
- [ ] Optional: Gallery images, testimonial photos

---

## FREE IMAGE RESOURCES

If you need stock photos:
- [Unsplash](https://unsplash.com) - Free high-quality photos
- [Pexels](https://pexels.com) - Free stock photos
- [Freepik](https://freepik.com) - Free with attribution

**Search terms:**
- Gym: "gym interior", "fitness training", "personal trainer"
- Spa: "spa massage", "wellness retreat", "aromatherapy"
- Wedding: "wedding photography", "bride groom", "wedding ceremony"
- Restaurant: "korean bbq", "grilled meat", "restaurant interior"
- Legal: "law office", "professional portrait", "business meeting"

---

## NEED HELP?

If you're stuck on a specific image replacement, just let me know which template and which section, and I'll give you the exact code to change!
