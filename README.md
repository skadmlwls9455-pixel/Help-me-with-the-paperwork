# 📄 Help Me With the Paperwork

> An open-source AI assistant that helps immigrants understand bureaucratic documents — through the messaging apps they already use.

---

## The Problem

Receiving an official letter from USCIS, the DMV, or a government agency is stressful.  
For immigrants who aren't fluent in English, it can be paralyzing.

**The existing solutions all have the same critical barriers:**

| Barrier | What it looks like |
|--------|-------------------|
| 🔒 Unfamiliarity | New apps require learning new interfaces |
| 🔍 Information gap | Many don't know AI tools like ChatGPT even exist |
| 😤 Convenience gap | Even if they know, switching tools is more friction than just calling their kid |

The result? Documents go ignored. Deadlines are missed. People pay lawyers for questions that could be answered clearly and simply.

---

## The Insight

**We don't need to build a new app.**  
We need to meet people where they already are.

| Community | Already using |
|-----------|--------------|
| Korean immigrants | KakaoTalk |
| Spanish-speaking immigrants | WhatsApp |
| Chinese immigrants | WeChat |
| General | SMS |

**Send a photo. Get a plain-language explanation. In your language. In the app you already use.**

No downloads. No accounts. No learning curve.

---

## How It Works

1. User sends a photo of an official document via their preferred messenger
2. AI reads the document and responds with:
   - What this document **is**
   - What it is **asking** from you
   - What you should **do next**
   - Whether you need professional help — with referrals to **free legal aid**
3. Response is delivered in the user's native language

---

## What It Doesn't Do

- ❌ Provide legal advice
- ❌ Fill out forms on your behalf  
- ❌ Make predictions about your case

Every response includes a clear disclaimer and, where relevant, a referral to free legal resources (legal aid societies, nonprofit immigration services, community centers).

---

## Architecture

```
User (KakaoTalk / WhatsApp / WeChat)
            ↓
   Messenger Webhook
            ↓
   Backend (Python / Node.js)
            ↓
     Claude API (Vision + Language)
            ↓
 Response in user's native language
```

---

## Roadmap

- [ ] MVP: KakaoTalk channel — Korean-American community
- [ ] WhatsApp integration — Spanish-speaking community  
- [ ] WeChat integration — Chinese-speaking community
- [ ] Web fallback for community centers and libraries
- [ ] Pilot partnerships with immigrant support NGOs

---

## Why Open Source?

This tool should be freely deployable by any organization that serves immigrant communities — community centers, legal aid nonprofits, libraries, churches, schools.

Open source means:
- Organizations can **verify** what the code does
- No vendor lock-in
- Community can extend it for their language and context

The goal isn't a product. It's infrastructure that belongs to the communities it serves.

---

## Contributing

This project is in early stages. Contributions especially welcome from:

- **Native speakers** who can review and improve prompts in their language
- **Developers** familiar with KakaoTalk / WhatsApp / WeChat APIs
- **Immigrant service organizations** interested in piloting

---

## License

MIT

---

*Built by [Katherine Nahm](https://github.com/skadmlwls9455-pixel)*  
*Inspired by the gap between the systems that exist and the people they were never designed for.*# Help-me-with-the-paperwork
