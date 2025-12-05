# 📘 HTML in CSS

Živjo! To stran sem naredila, da hitro najdeš značko, ki jo potrebuješ. Upam, da ti bo koristilo in veliko uspeha pri grajenju strani. 🎉

---

# 📑 Kazalo

1. [Osnovna HTML struktura](#osnovna-html-struktura)
2. [Naslovi](#naslovi)
3. [Odstavki](#odstavki)
4. [Urejanje besedila](#urejanje-besedila)
5. [Linki](#linki)
6. [Barve v CSS](#barve-v-css)
7. [Primeri za kopiranje](#primeri-za-kopiranje)

---

# 🧩 Osnovna HTML struktura

```html
<!DOCTYPE html>
<html>
<head>
    <title>Moja stran</title>
</head>
<body>
    <h1>Živjo!</h1>
</body>
</html>
```

---

# Naslovi
```html
<h1>Največji naslov</h1>
<h2>Malo manjši</h2>
<h3>Še malo manjši</h3>
<h4>Še še manjši</h4>
<h5>Že zelo majhen</h5>
<h6>Najmanjši naslov</h6>
```

# Odstavki

```html
<p>To je besedilo.</p>
```

# Urejanje besedila

```html
<br> -> Gre v novo vrstico.
<hr> -> Naredi črto čez stran
```
```html
<b>Odebeljeno besedilo</b>
<strong>Pomebno besedilo</strong>
<i>italic/poševno besedilo</i>
<u>Podčrtano besedilo</u>
<del>Prečrtano besedilo</del>
<mark>Označeno z barvo</mark>
```

# Linki

```html
<a href="url">link text</a>
```
Atribut target
- _self -> Odpre v istem zavihku, kjer se nahajamo
```html
<a href="url" target="_self">link text</a>
```
- _blank -> Odpre v novem zavihku (Zmeraj priporočam!!!)
```html
<a href="url" target="_blank">link text</a>
```
### Kako uporabimo sliko kot link?
```html
<a href="default.asp">
<img src="smiley.gif" alt="HTML tutorial"">
</a>
```
---

# 🎨 Kaj je CSS?

CSS je jezik za barve, velikosti in videz na spletni strani. Kot barvice za HTML.

---

# 🖍️ Kako dodamo CSS?

### Najlažje:

```html
<style>
    body {
        background-color: lightblue;
    }
</style>
```

---

# 🌈 Najpogostejša CSS pravila

### Barva ozadja

```css
background-color: yellow;
```

### Barva besedila

```css
color: red;
```

### Velikost besedila

```css
font-size: 24px;
```

### Poravnava

```css
text-align: center;
```

---

# 🎨 Barve v CSS

Lahko uporabljaš besede ali HEX kode.

### Primeri

```css
color: blue;
color: #ff5733; /* oranžna */
```

---

# 💡 Primeri za kopiranje

## Preprost naslov in paragraf

```html
<h1>Moj naslov</h1>
<p>To je moja prva HTML vrstica!</p>
```

## Barvno ozadje strani

```html
<style>
body {
    background-color: pink;
}
</style>
```
