# Masomo Yangu - Tovuti ya Mafunzo

Website rahisi na safi ya kuweka masomo yako. Inaweza kuwekwa kwenye **Netlify** bure.

---

## 📁 Muundo wa Folda

```
masomo-website/
├── index.html              ← Ukurasa mkuu (orodha ya masomo)
├── css/
│   └── styles.css          ← Muonekano (design)
├── js/
│   ├── lessons-data.js     ← ORODHA YA MASOMO (ongeza hapa)
│   └── script.js
├── masomo/
│   ├── somo-01.html        ← Somo la kwanza
│   ├── somo-02.html        ← Somo la pili
│   └── ...                 ← Ongeza masomo mengine hapa
├── assets/
│   ├── images/             ← Picha
│   ├── videos/             ← Video (ikiwa utapakia moja kwa moja)
│   └── audio/              ← Faili za sauti/muziki (.mp3)
└── README.md
```

---

## 🚀 Jinsi ya Kuongeza Somo Jipya (Hatua kwa Hatua)

### Hatua 1: Ongeza kwenye orodha
Fungua faili `js/lessons-data.js` na ongeza somo jipya kama hivi:

```js
{
  id: "03",
  title: "Jina la Somo Lako",
  description: "Maelezo mafupi ya somo hili...",
  file: "masomo/somo-03.html",
  date: "2025-02-10"
},
```

### Hatua 2: Unda faili la somo
1. Nakili faili `masomo/somo-01.html`
2. Ipe jina jipya: `somo-03.html`
3. Fungua na ubadilishe:
   - Kichwa cha somo
   - Maandishi
   - HTML yoyote unayotaka
   - Link ya video (YouTube)
   - Faili la sauti (ikiwa lipo)

### Hatua 3: Hifadhi na upelekе kwenye Netlify
Baada ya kuhifadhi, fuata maelekezo ya kupeleka hapa chini.

---

## 📤 Jinsi ya Kupeleka kwenye Netlify + GitHub

### Njia A: Kupitia GitHub (Inapendekezwa)

1. **Unda akaunti** kwenye [GitHub.com](https://github.com) (bure)
2. Bofya **New repository**
   - Jina: `masomo-yangu` (au jina lolote)
   - Chagua **Public**
   - Usichague "Add README"
3. Pakia folda yote ya `masomo-website`:
   - Unaweza kutumia GitHub Desktop (rahisi) au drag & drop faili kwenye tovuti ya GitHub
4. Nenda kwenye [Netlify.com](https://www.netlify.com) → Jisajili (bure)
5. Bofya **Add new site** → **Import an existing project**
6. Chagua **GitHub** na ruhusu Netlify
7. Chagua repository yako (`masomo-yangu`)
8. Settings:
   - Build command: (acha tupu)
   - Publish directory: `/` (au `.`)
9. Bofya **Deploy site**
10. Baada ya dakika chache utapata link kama:
    `https://random-name-123.netlify.app`

Unaweza kubadilisha jina la link kwenye **Site settings → Domain management**.

### Njia B: Drag & Drop (Haraka sana kwa mwanzo)

1. Nenda kwenye [app.netlify.com/drop](https://app.netlify.com/drop)
2. Buruta folda yote ya `masomo-website` na uiache pale
3. Utapata link mara moja

**Kumbuka:** Njia hii ni rahisi lakini kila unapobadilisha kitu unahitaji kurudia drag & drop. Njia ya GitHub ni bora zaidi kwa siku zijazo.

---

## 🎥 Jinsi ya Kuweka Video

### Njia bora: YouTube
1. Pakia video yako kwenye YouTube (unaweza kuweka "Unlisted")
2. Bofya **Share → Embed**
3. Nakili namba ya video (mfano: `dQw4w9WgXcQ`)
4. Weka kwenye faili la somo:

```html
<iframe 
  src="https://www.youtube.com/embed/NAMBA_YA_VIDEO" 
  title="Video ya Somo"
  frameborder="0" 
  allowfullscreen>
</iframe>
```

### Njia nyingine: Faili moja kwa moja
Weka faili la video ndani ya `assets/videos/` kisha:

```html
<video controls>
  <source src="../assets/videos/jina-la-video.mp4" type="video/mp4">
</video>
```

(Video kubwa zinaweza kufanya site iwe nzito. YouTube ni bora zaidi.)

---

## 🎵 Jinsi ya Kuweka Sauti / Muziki

1. Weka faili lako la `.mp3` ndani ya folda `assets/audio/`
2. Kwenye faili la somo andika:

```html
<audio controls>
  <source src="../assets/audio/jina-la-faili.mp3" type="audio/mpeg">
</audio>
```

---

## 💡 Vidokezo Muhimu

- Kila unapoongeza somo jipya, kumbuka kulisajili kwenye `js/lessons-data.js`
- Unaweza kubadilisha rangi na muonekano kwa kuhariri `css/styles.css`
- Website hii inafanya kazi vizuri kwenye simu na kompyuta
- Hakuna haja ya database wala server — yote ni static

---

Imeundwa kwa ajili yako.  
Furahia kuweka masomo yako!
