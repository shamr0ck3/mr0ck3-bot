# 🤖 MR0CK3 AI Bot

Floating cyberpunk chatbot widget for Blogspot, powered by a live `pages.json` file.

---

## 📁 Files

| File | Purpose |
|------|---------|
| `index.html` | The bot widget (push this, never touch again) |
| `pages.json` | Your blog data — **edit this to add new posts** |

---

## 🚀 Deploy to GitHub Pages

1. Push both files to this repo (`mr0ck3-bot`)
2. Go to **Settings → Pages → Source: main / root**
3. Bot is live at `https://shamr0ck3.github.io/mr0ck3-bot/`

---

## ✏️ Adding a New Blog Post

Open `pages.json` and add to the `posts` array:

```json
{
  "title": "My New Post Title",
  "url": "https://10kfollowerschallenge.blogspot.com/YOUR-POST-URL",
  "category": "tutorial",
  "description": "Short description shown in bot"
}
```

**Available categories:** `tutorial` · `project` · `tool` · `growth` · `main`

Push → bot instantly shows the new post. ✅

---

## 🧩 Embed into Blogspot

**Blogger → Theme → Edit HTML → paste before `</body>`:**

```html
<iframe
  src="https://shamr0ck3.github.io/mr0ck3-bot/"
  style="position:fixed;bottom:0;right:0;width:420px;height:640px;border:none;z-index:99999;background:transparent;"
  scrolling="no" frameborder="0" allowtransparency="true">
</iframe>
```

---

## 💡 Tips

- Post categories appear as **quick-reply chips** automatically
- Add new categories in the `categories` array in `pages.json`
- Bot fetches fresh data every time it loads (cache-busted)
