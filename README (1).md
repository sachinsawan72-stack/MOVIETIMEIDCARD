# Platinum – Movie Time Cinemas Employee ID Card

Ek single-file HTML ID card (front + back). Koi installation ya internet ki zarurat nahi.

## Files

| File | Kaam |
|------|------|
| `id-card.html` | Poora ID card. Isko browser mein kholein. |
| `README.md` | Ye guide. |

## Kaise kholein

1. `id-card.html` par double-click karein (Chrome, Edge, Firefox ya Safari mein khulega).
2. Mobile par bhi browser mein khul jata hai.

## Features

- **Front aur back** dono side ek hi page par.
- **Sab text editable:** Kisi bhi text par click karke type karein.
  - Front: Logo naam, tagline, Name, Post, Emp Code, Issuing Authority.
  - Back: Emergency Contact, Blood Group, "If found please return to", company naam, address, phone, website.
- **Logo aur tagline sync:** Front par badlenge to back par bhi apne aap badal jayenge.
- **Photo upload (passport size 3.5 x 4.5 cm):**
  - Toolbar ka "Photo upload karein" button, photo box par click, ya drag and drop.
  - Photo apne aap 3.5 : 4.5 ratio mein crop hoti hai.
  - "Photo download" se crop ki hui photo 413 x 531 px (300 dpi) JPG mein save hoti hai.
  - "Photo hatayein" se photo hat jati hai.
- **Signature upload (Issuing Authority):**
  - Toolbar ka "Signature upload karein" button, ya signature box par click.
  - White background wali signature image bhi saaf dikhti hai.
  - "Signature hatayein" se hata sakte hain.
- **Rang badalna:** Toolbar mein Blue, Orange aur Company name ke color picker.
- **Print / PDF:** "Print / PDF" button se card print karein ya PDF mein save karein.

## Print karne ke tips

1. "Print / PDF" dabayein.
2. Print window mein **Background graphics** option ON rakhein, taaki neeli aur orange patti print ho.
3. Scale 100% rakhein.
4. PDF chahiye to destination mein "Save as PDF" chunein.
5. Card ka size screen par 320 x 512 px hai. Asli PVC card size (CR80, 54 x 86 mm) ke liye printer ya print shop mein scale adjust karwa lein.

## Zaroori baatein

- **Edits save nahi hote.** Page refresh ya band karne par sab kuch pehle jaisa ho jata hai. Pehle print ya PDF save kar lein.
- **Logo text-based hai.** Asli Platinum logo ki jagah font se bana hua logo hai. Asli logo (PNG/SVG) ho to usse replace kiya ja sakta hai.
- **Photo aur signature** sirf aapke browser mein rehte hain. Kahin upload nahi hote.
- Sirf image files (JPG, PNG, WEBP) chalti hain.

## Code mein badlav (optional)

`id-card.html` ke upar `<style>` section mein:

| Kya badalna hai | Kahan |
|-----------------|-------|
| Default colors | `:root{--blue:...; --orange:...; --red:...}` |
| Photo box ka size | `.photo{width:140px; height:180px}` (ratio 7 : 9 rakhein) |
| Name / Post / Emp Code ki jagah | `.details{top:330px}` |
| Card ka size | `.card{width:320px; height:512px}` |
| Default text (naam, address, phone) | `<body>` ke andar HTML mein seedha |
