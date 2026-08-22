# 🗿 lordmega baileys

[![Logo](https://files.catbox.moe/7vx45a.png)](https://www.npmjs.com/package/@lordmega/baileys)

<p align="center">
   Mega enhanced Baileys v7 with newsletter media upload fixes, interactive messages, album support, and extended message type coverage.
   <br><br>
   <a href="https://www.npmjs.com/package/@lordmega/baileys">
      <img src="https://img.shields.io/npm/v/@lordmega/baileys?style=for-the-badge&logo=npm"/>
   </a>
   <a href="https://www.npmjs.com/package/@lordmega/baileys">
      <img src="https://img.shields.io/npm/dm/@lordmega/baileys?style=for-the-badge&logo=npm"/>
   </a>
   <a href="https://github.com/lordmega/baileys">
      <img src="https://img.shields.io/github/stars/lordmega/baileys?style=for-the-badge&logo=github"/>
   </a>
   <a href="LICENSE">
      <img src="https://img.shields.io/badge/license-MIT-blue?style=for-the-badge"/>
   </a>
   <a href="https://nodejs.org">
      <img src="https://img.shields.io/badge/node-%3E%3D20-339933?logo=node.js&labelColor=green&logoColor=white&style=for-the-badge"/>
   </a>
   <a href="#">
      <img src="https://img.shields.io/badge/ESM-only?logo=javascript&labelColor=yellow&logoColor=black&style=for-the-badge"/>
   </a>
</p>

### 📋 Table of Contents
- [📋 Table of Contents](#-table-of-contents)
- [✨ Highlights](#-highlights)
- [🛠️ Internal Adjustments](#%EF%B8%8F-internal-adjustments)
- [📨 Messages Handling & Compatibility](#-messages-handling--compatibility)
- [🧩 Additional Message Options](#-additional-message-options)
- [🚀 Try the Bot](#-try-the-bot)
- [📦 Fork Base](#-fork-base)

---

### ✨ Highlights

Built for production with an emphasis on readability and reliability:

- 🚫 No obfuscation — clean, auditable code.
- 🚫 No auto-follow channel (newsletter) behavior.
- 👁️ Reveal view-once messages via `sock.rvo()`.
- 📱 Android browser support to receive view-once messages.
- ✏️ Automatic decryption of E2EE message edits (May 2026+).
- 🔑 Caller-supplied `messageSecret` support on any message type.

### 🛠️ Internal Adjustments

- 🖼️ Fixed newsletter media upload failures caused by an upstream bug.
- 📁 Restored `makeInMemoryStore` with a lightweight ESM adaptation and minor compatibility tweaks for Baileys v7.
- 📦 Replaced FFmpeg `exec` calls with `spawn` for more reliable process management.
- 🗃️ Added [`@napi-rs/image`](https://www.npmjs.com/package/@napi-rs/image) as a supported backend in `getImageProcessingLibrary()`, providing a solid balance between speed and compatibility.
- 🔒 Spoofing guards on self-only protocol messages.

### 📨 Messages Handling & Compatibility

- 📩 Extended message type support for:
   - 🖼️ Album Message
   - 👤 Group Status Message
   - 👉🏻 Interactive Message (buttons, lists, native flows, templates, carousels)
   - 🎞️ Status Mention Message
   - 📦 Sticker Pack Message
   - ✨ Rich Response Message **[NEW]**
   - 🧾 Message with Code Blocks **[NEW]**
   - 🌏 Message with Inline Entities **[NEW]**
   - 📋 Message with Table **[NEW]**
   - 💳 Payment-related Messages (requests, invites, orders, invoices)
- 📰 Simplified ad thumbnail sending via `externalAdReply` — no manual `contextInfo` required.
- 💭 Added support for quoting messages inside newsletters. **[NEW]**
- 🎀 Added support for custom button icons. **[NEW]**
- 👁️ Reveal view-once messages and resend as normal media via `sock.rvo()`. **[NEW]**

### 🧩 Additional Message Options

- 👁️ Optional boolean flags for message behavior:
   - 🤖 `ai` — AI icon on message
   - 📣 `mentionAll` — Mention all group participants without specifying individual JIDs **[NEW]**
   - 🔧 `ephemeral`, `groupStatus`, `isLottie`, `spoiler`, `viewOnce`, `viewOnceV2`, `viewOnceV2Extension`, `interactiveAsTemplate` — Message wrappers
   - 🔒 `secureMetaServiceLabel` — Secure meta service label **[NEW]**
   - 📄 `raw` — Build message proto manually **(DO NOT USE FOR EXPLOITATION)**
- 🔑 Pass a custom 32-byte `messageSecret` on any message type via send options.

---

### 🚀 Try the Bot

A lightweight, modular WhatsApp bot built on this library — includes group management, moderation, quiz games, and utility tools.

👉🏻 [MegaBot MD](https://github.com/LORDMEGA-MD/MEGABOT5)

---

### 📦 Fork Base

Based on [WhiskeySockets/Baileys](https://github.com/WhiskeySockets/Baileys)

