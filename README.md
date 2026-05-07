<div align="center">

# 🎮 kick-stream

<p align="center">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/>
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white"/>
  <img src="https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white"/>
</p>

<p align="center">
  <img src="https://img.shields.io/github/stars/abdulrahmanqdev/kick-stream?style=flat-square&color=yellow"/>
  <img src="https://img.shields.io/github/forks/abdulrahmanqdev/kick-stream?style=flat-square&color=green"/>
  <img src="https://img.shields.io/github/last-commit/abdulrahmanqdev/kick-stream?style=flat-square&color=orange"/>
  <img src="https://img.shields.io/npm/v/kick-stream?style=flat-square&color=red"/>
  <img src="https://img.shields.io/npm/dm/kick-stream?style=flat-square&color=blue"/>
</p>

<p align="center">
  <strong>Kick.com platformu için hafif ve kullanımı kolay Node.js paketi.</strong><br/>
  Yayıncı bilgisi, yayın verisi ve URL çözücü — tek pakette.
</p>

</div>

---

## 📦 Kurulum

```bash
npm install kick-stream
```

---

## 🚀 Kullanım

### Yayıncı Bilgisi Alma

```js
const kickClient = require('kick-stream');

const streamer = await kickClient.getStreamer('slow3rxq') // Yayıncı Adı
console.log(streamer) //{...} Yayıncı Verisi
```

### Yayın Verisi Alma

```js
const kickClient = require('kick-stream');

const stream = await kickClient.getStream('slow3rxq') // Yayıncı Adı
console.log(stream) //{...} Yayın Verisi
```

### Kick URL Çözücü (Opsiyonel)

Kick URL'sinden direkt kullanıcı adı çözümleyebilirsin:

```js
const kickClient = require('kick-stream')

console.log(kickClient.solveURL('https://kick.com/slow3rxq')) // "slow3rxq"
```

---

## 📖 API Referansı

| Metot | Parametre | Açıklama |
|---|---|---|
| `getStreamer(username)` | `string` | Yayıncı profil verisini döndürür |
| `getStream(username)` | `string` | Aktif yayın verisini döndürür |
| `solveURL(url)` | `string` | Kick URL'sinden kullanıcı adını çıkarır |

---

## ✨ Özellikler

- 📡 Yayıncı profil verisi çekme
- 🎥 Aktif yayın bilgisi alma
- 🔗 Kick URL'sinden kullanıcı adı çözümleme
- ⚡ Hafif ve sıfır bağımlılık
- 🟢 Promise / async-await desteği

---

## 👤 Geliştirici

**@abdulrahmanqdev**
