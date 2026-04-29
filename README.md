# 🚀 Netlify Relay (Edge Function)

> ⚡ A lightweight relay/proxy built with **Netlify Edge Functions**
> Created by **amirs**

---

## 🌐 Demo

After deployment:

```
https://your-site.netlify.app
```

---

## ✨ Features

* ⚡ Edge Functions (super fast)
* 🔁 Full request relay (proxy)
* 🌍 Works globally via Netlify CDN
* 🔒 Environment-based target config
* 🧩 Minimal & simple structure

---

## 📦 Project Structure

```
.
├── netlify/
│   └── edge-functions/
│       └── relay.js
├── public/
│   └── index.html
├── netlify.toml
├── package.json
```

---

## ⚙️ Environment Variable

You MUST set this:

```
TARGET_DOMAIN=https://example.com
```

---

## 🚀 Deploy (Netlify UI)

1. Go to https://app.netlify.com
2. Click **Add new project**
3. Import your GitHub repo
4. Set:

```
Build command: npm run build
Publish directory: public
```

5. Add Environment Variable:

```
TARGET_DOMAIN=https://your-domain.com
```

6. Deploy 🎉

---

## 💻 Deploy via CLI

```bash
npm install -g netlify-cli
netlify login
netlify init
netlify deploy --prod
```

---

## 🧪 Testing

Open:

```
https://your-site.netlify.app
```

Requests will be forwarded to your target domain.

---

## ⚠️ Notes

* Only use with domains you own or have permission to use
* Misuse may violate service policies

---

## 👤 Author

**amirs**

---

## 📜 License

MIT License © amirs
