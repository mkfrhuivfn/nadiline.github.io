# NADI LINE Photography Website
## ဖိုင်တွေဘယ်နေရာမှာ ထားရမလဲ (Folder Guide)

---

### 📁 Folder Structure (ဖိုင် ဖွဲ့စည်းပုံ)

```
nadi-photography/
│
├── index.html          ← Home Page (ပထမဆုံး ပေါ်လာမည့် page)
├── about.html          ← About Me Page
├── gallery.html        ← Photo Gallery Page
├── contact.html        ← Contact Page
│
├── css/
│   └── style.css       ← Website ရဲ့ အသွင်အပြင် (လုံးဝ မပြင်ဖို့ မဟုတ်ဘဲ)
│
├── js/
│   └── main.js         ← Website ရဲ့ လုပ်ဆောင်ချက်များ
│
└── images/
    ├── gallery/        ← ဒီနေရာမှာ Gallery ဓာတ်ပုံများ ထည့်ပါ
    │   ├── photo1.jpg
    │   ├── photo2.jpg
    │   ├── photo3.jpg
    │   └── ... (ဆက်ထည့်နိုင်သည်)
    │
    └── about/
        └── portrait.jpg  ← ဒီနေရာမှာ မိမိ ကိုယ်တိုင်ရဲ့ ဓာတ်ပုံ ထည့်ပါ
```

---

### 🖼️ ဓာတ်ပုံ ထည့်နည်း (How to Add Photos)

#### Gallery ဓာတ်ပုံများ:
1. သင်ရိုက်ထားသော ဓာတ်ပုံများကို **images/gallery/** folder ထဲသို့ ထည့်ပါ
2. ဖိုင်အမည်များကို `photo1.jpg`, `photo2.jpg` ... ဟု နာမည်ပေးပါ
   သို့မဟုတ် ကိုယ်ပိုင် နာမည်ပေးနိုင်သည် (ဥပမာ `phuket-beach.jpg`)
3. **gallery.html** ဖိုင်ကိုဖွင့်ပြီး ဤ section ကို ရှာပါ:
   ```html
   <div class="gallery-item" data-category="coast">
     <img src="images/gallery/photo1.jpg" alt="Phuket Coastline" .../>
   ```
   - `photo1.jpg` နေရာတွင် သင်၏ ဓာတ်ပုံ ဖိုင်အမည် ဖြည့်ပါ
   - `alt=""` ထဲတွင် ဓာတ်ပုံ ဖော်ပြချက် ဖြည့်ပါ (SEO အတွက် အရေးကြီး)
   - `data-category=` တွင် အောက်ပါ category ၄ ခုမှ ရွေးပါ:
     - `coast` = ကမ်းရိုးတန်း ဓာတ်ပုံ
     - `nature` = သဘာဝ / သစ်ပင်
     - `wildlife` = တိရိစ္ဆာန်
     - `golden` = နေဝင်ချိန် / မနက်ခင်း

#### Hero (Home Page ကြီးကြီးမားမား ဓာတ်ပုံ):
**css/style.css** ဖိုင်ကိုဖွင့်ပြီး ဤ line ကို ရှာပါ:
```css
.hero-bg {
  /* background-image: url('../images/gallery/hero.jpg'); */
```
`/* */` ကို ဖြုတ်ပြီး သင့် ဓာတ်ပုံ path ဖြည့်ပါ:
```css
background-image: url('../images/gallery/hero.jpg');
```

#### ကိုယ်တိုင် ပုံ (About Page):
- **images/about/** folder ထဲသို့ `portrait.jpg` ဟု နာမည်ပေးထည့်ပါ

---

### ✏️ ကိုယ်ပိုင် အချက်အလက် ဖြည့်နည်း

**about.html** ဖိုင်တွင်:
- `Hello, I'm Nadi` → မိမိ နာမည် ဖြည့်ပါ
- paragraph (`<p>`) tags အတွင်း မိမိ အကြောင်း ရေးပါ

**contact.html** ဖိုင်တွင်:
- `hello@nadilinephoto.com` → မိမိ email ဖြည့်ပါ
- `@nadilinephotography` → မိမိ Instagram ဖြည့်ပါ

---

### 🌐 GitHub Pages တင်နည်း

1. GitHub.com တွင် repository တစ်ခု ဖန်တီးပါ
2. ဖိုင်အားလုံးကို upload လုပ်ပါ
3. Settings → Pages → Source: main branch ရွေးပါ
4. Website URL: `https://yourusername.github.io/repo-name`

---

### 📱 Mobile Friendly

ဤ website သည် phone, tablet, computer အားလုံးတွင် အလုပ်လုပ်ပါသည်။
CSS ထဲတွင် responsive design ပါဝင်ပြီးဖြစ်ပါသည်။

---

*Nadi Line Photography © 2026 | Built with ♥*
