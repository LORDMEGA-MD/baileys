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
- [📥 Installation](#-installation)
   - [🧩 Import (ESM & CJS)](#-import-esm--cjs)
- [🚀 Quick Start](#-quick-start)
- [🌐 Connect to WhatsApp (Quick Step)](#-connect-to-whatsapp-quick-step)
   - [🔐 Auth State](#-auth-state)
- [🗄️ Implementing Data Store](#%EF%B8%8F-implementing-data-store)
- [🪪 WhatsApp IDs Explain](#-whatsapp-ids-explain)
- [✉️ Sending Messages](#%EF%B8%8F-sending-messages)
   - [🔠 Text](#-text)
   - [🔔 Mention](#-mention)
   - [😁 Reaction](#-reaction)
   - [📌 Pin Message](#-pin-message)
   - [🔖 Keep Chat](#-keep-chat)
   - [➡️ Forward Message](#%EF%B8%8F-forward-message)
   - [👤 Contact](#-contact)
   - [📍 Location](#-location)
   - [🗓️ Event](#%EF%B8%8F-event)
   - [👥 Group Invite](#-group-invite)
   - [🛍️ Product](#%EF%B8%8F-product)
   - [📊 Poll](#-poll)
   - [💭 Button Response](#-button-response)
   - [✨ Rich Response](#-rich-response)
   - [🧾 Message with Code Block](#-message-with-code-block)
   - [🌏 Message with Inline Entities](#-message-with-inline-entities)
   - [📋 Message with Table](#-message-with-table)
   - [🎞️ Status Mention](#%EF%B8%8F-status-mention)
- [📁 Sending Media Messages](#-sending-media-messages)
   - [🖼️ Image](#%EF%B8%8F-image)
   - [🎥 Video](#-video)
   - [📃 Sticker](#-sticker)
   - [💽 Audio](#-audio)
   - [🗂️ Document](#%EF%B8%8F-document)
   - [🖼️ Album (Image & Video)](#%EF%B8%8F-album-image--video)
   - [📦 Sticker Pack](#-sticker-pack)
- [👁️ Reveal View-Once](#%EF%B8%8F-reveal-view-once)
- [👉🏻 Sending Interactive Messages](#-sending-interactive-messages)
   - [🔘 Buttons](#-buttons)
   - [📋 List](#-list)
   - [🗄️ Interactive](#%EF%B8%8F-interactive)
   - [🫙 Hydrated Template](#-hydrated-template)
- [💳 Sending Payment Messages](#-sending-payment-messages)
   - [➕ Invite Payment](#-invite-payment)
   - [🧾 Invoice](#-invoice)
   - [🛍️ Order](#%EF%B8%8F-order)
   - [💳 Request Payment](#-request-payment)
- [👁️ Other Message Options](#%EF%B8%8F-other-message-options)
   - [🤖 AI Icon](#-ai-icon)
   - [🕒 Ephemeral](#-ephemeral)
   - [📰 External Ad Reply](#-external-ad-reply)
   - [🧑‍🧑‍🧒 Group Status](#%E2%80%8D%E2%80%8D-group-status)
   - [🐱 Lottie Sticker](#-lottie-sticker)
   - [🧩 Raw](#-raw)
   - [🏷️ Secure Meta Service Label](#%EF%B8%8F-secure-meta-service-label)
   - [📑 Spoiler](#-spoiler)
   - [👁️ View Once](#%EF%B8%8F-view-once)
   - [👁️ View Once V2](#%EF%B8%8F-view-once-v2)
   - [👁️ View Once V2 Extension](#%EF%B8%8F-view-once-v2-extension)
- [♻️ Modify Messages](#%EF%B8%8F-modify-messages)
   - [🗑️ Delete Messages](#%EF%B8%8F-delete-messages)
   - [✏️ Edit Messages](#%EF%B8%8F-edit-messages)
- [🧰 Additional Contents](#-additional-contents)
   - [🏷️ Find User ID (JID|PN/LID)](#%EF%B8%8F-find-user-id-jidpnlid)
   - [🔑 Request Custom Pairing Code](#-request-custom-pairing-code)
   - [🖼️ Image Processing](#%EF%B8%8F-image-processing)
   - [📣 Newsletter Management](#-newsletter-management)
   - [👥 Group Management](#-group-management)
   - [👥 Community Management](#-community-management)
   - [👤 Profile Management](#-profile-management)
   - [🛒 Business Management](#-business-management)
   - [🔐 Privacy Management](#-privacy-management)
   - [📡 Events](#-events)
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
- 🗃️ Added [`@napi-rs/image`](https://www.npmjs.com/package/@napi-rs/image) as a supported backend in [`getImageProcessingLibrary()`](#%EF%B8%8F-image-processing), providing a solid balance between speed and compatibility.
- 🔒 Spoofing guards on self-only protocol messages.

### 📨 Messages Handling & Compatibility

- 📩 Extended message type support for:
   - 🖼️ [Album Message](#%EF%B8%8F-album-image--video)
   - 👤 [Group Status Message](#%E2%80%8D%E2%80%8D-group-status)
   - 👉🏻 [Interactive Message](#-sending-interactive-messages) (buttons, lists, native flows, templates, carousels)
   - 🎞️ [Status Mention Message](#%EF%B8%8F-status-mention)
   - 📦 [Sticker Pack Message](#-sticker-pack)
   - ✨ [Rich Response Message](#-rich-response) **[NEW]**
   - 🧾 [Message with Code Blocks](#-message-with-code-block) **[NEW]**
   - 🌏 [Message with Inline Entities](#-message-with-inline-entities) **[NEW]**
   - 📋 [Message with Table](#-message-with-table) **[NEW]**
   - 💳 [Payment-related Messages](#-sending-payment-messages) (requests, invites, orders, invoices)
- 📰 Simplified ad thumbnail sending via [`externalAdReply`](#-external-ad-reply) — no manual `contextInfo` required.
- 💭 Added support for quoting messages inside newsletters. **[NEW]**
- 🎀 Added support for [custom button icons](#%EF%B8%8F-interactive). **[NEW]**
- 👁️ Reveal view-once messages and resend as normal media via [`sock.rvo()`](#%EF%B8%8F-reveal-view-once). **[NEW]**

### 🧩 Additional Message Options

- 👁️ Optional boolean flags for message behavior:
   - 🤖 [`ai`](#-ai-icon) — AI icon on message
   - 📣 [`mentionAll`](#-mention) — Mention all group participants without specifying individual JIDs **[NEW]**
   - 🔧 [`ephemeral`](#-ephemeral), [`groupStatus`](#%E2%80%8D%E2%80%8D-group-status), [`isLottie`](#-lottie-sticker), [`spoiler`](#-spoiler), [`viewOnce`](#%EF%B8%8F-view-once), [`viewOnceV2`](#%EF%B8%8F-view-once-v2), [`viewOnceV2Extension`](#%EF%B8%8F-view-once-v2-extension), [`interactiveAsTemplate`](#%EF%B8%8F-interactive) — Message wrappers
   - 🔒 [`secureMetaServiceLabel`](#%EF%B8%8F-secure-meta-service-label) — Secure meta service label **[NEW]**
   - 📄 [`raw`](#-raw) — Build message proto manually **(DO NOT USE FOR EXPLOITATION)**
- 🔑 Pass a custom 32-byte `messageSecret` on any message type via send options.

---

### 📥 Installation

- 📄 Via `package.json`

```json
# NPM
"dependencies": {
   "@lordmega/baileys": "latest"
}

# GitHub
"dependencies": {
   "@lordmega/baileys": "github:lordmega/baileys"
}
```

- ⌨️ Via terminal

```bash
# NPM
npm i @lordmega/baileys@latest

# GitHub
npm i github:lordmega/baileys
```

#### 🧩 Import (ESM & CJS)

```javascript
// --- ESM
import { makeWASocket } from '@lordmega/baileys'

// --- CJS (tested and working on Node.js 24 ✅)
const { makeWASocket } = require('@lordmega/baileys')
```

---

### 🚀 Quick Start

```javascript
import { makeWASocket, useMultiFileAuthState, DisconnectReason } from '@lordmega/baileys'
import { Boom } from '@hapi/boom'

const { state, saveCreds } = await useMultiFileAuthState('auth')

const sock = makeWASocket({ auth: state, printQRInTerminal: true })

sock.ev.on('creds.update', saveCreds)

sock.ev.on('connection.update', ({ connection, lastDisconnect }) => {
  if (connection === 'close') {
    const reconnect = lastDisconnect?.error?.output?.statusCode !== DisconnectReason.loggedOut
    if (reconnect) makeWASocket({ auth: state })
  }
})

sock.ev.on('messages.upsert', async ({ messages }) => {
  const msg = messages[0]
  if (!msg.key.fromMe && msg.message?.conversation) {
    await sock.sendMessage(msg.key.remoteJid, { text: 'pong' })
  }
})
```

---

### 🌐 Connect to WhatsApp (Quick Step)

```javascript
import { makeWASocket, delay, DisconnectReason, useMultiFileAuthState } from '@lordmega/baileys'
import { Boom } from '@hapi/boom'
import pino from 'pino'

const myPhoneNumber = '2560000000'

const logger = pino({ level: 'silent' })

const connectToWhatsApp = async () => {
   const { state, saveCreds } = await useMultiFileAuthState('session')
    
   const sock = makeWASocket({
      logger,
      auth: state
   })

   sock.ev.on('creds.update', saveCreds)

   sock.ev.on('connection.update', (update) => {
      const { connection, lastDisconnect } = update
      if (connection === 'connecting' && !sock.authState.creds.registered) {
         await delay(1500)
         const code = await sock.requestPairingCode(myPhoneNumber)
         console.log('🔗 Pairing code', ':', code)
      }
      else if (connection === 'close') {
         const shouldReconnect = new Boom(connection?.lastDisconnect?.error)?.output?.statusCode !== DisconnectReason.loggedOut
         console.log('⚠️ Connection closed because', lastDisconnect.error, ', reconnecting ', shouldReconnect)
         if (shouldReconnect) {
            connectToWhatsApp()
         }
      }
      else if (connection === 'open') {
         console.log('✅ Successfully connected to WhatsApp')
      }
   })

   sock.ev.on('messages.upsert', async ({ messages }) => {
      for (const message of messages) {
         if (!message.message) continue

         console.log('🔔 Got new message', ':', message)
         await sock.sendMessage(message.key.remoteJid, {
            text: '👋🏻 Hello world'
         })
      }
   })
}

connectToWhatsApp()
```

#### 🔐 Auth State

> [!NOTE]
> You can use the experimental `useSingleFileAuthState` and `useSqliteAuthState` as alternatives to `useMultiFileAuthState`. Note that `useSingleFileAuthState` has built-in caching, so wrapping `state.keys` with `makeCacheableSignalKeyStore` is unnecessary.

#### 📱 Android Browser (receive view-once)

Connect as an Android client to receive view-once messages natively:

```javascript
import { makeWASocket, Browsers } from '@lordmega/baileys'

const sock = makeWASocket({ auth: state, browser: Browsers.android('Chrome') })
```

---

### 🗄️ Implementing Data Store

> [!CAUTION]
> Building your own data store is strongly recommended — keeping full chat history in memory can cause excessive RAM usage.

```javascript
import { makeWASocket, makeInMemoryStore, delay, DisconnectReason, useMultiFileAuthState } from '@lordmega/baileys'
import { Boom } from '@hapi/boom'
import pino from 'pino'

const myPhoneNumber = '6288888888888'
const storePath = './store.json'
const logger = pino({ level: 'silent' })

const connectToWhatsApp = async () => {
   const { state, saveCreds } = await useMultiFileAuthState('session')
    
   const sock = makeWASocket({
      logger,
      auth: state
   })

   const store = makeInMemoryStore({
      logger,
      socket: sock
   })

   store.bind(sock.ev)

   sock.ev.on('creds.update', saveCreds)

   sock.ev.on('connection.update', (update) => {
      const { connection, lastDisconnect } = update
      if (connection === 'connecting' && !sock.authState.creds.registered) {
         await delay(1500)
         const code = await sock.requestPairingCode(myPhoneNumber)
         console.log('🔗 Pairing code', ':', code)
      }
      else if (connection === 'close') {
         const shouldReconnect = new Boom(connection?.lastDisconnect?.error)?.output?.statusCode !== DisconnectReason.loggedOut
         console.log('⚠️ Connection closed because', lastDisconnect.error, ', reconnecting ', shouldReconnect)
         if (shouldReconnect) {
            connectToWhatsApp()
         }
      }
      else if (connection === 'open') {
         console.log('✅ Successfully connected to WhatsApp')
      }
   })

   sock.ev.on('chats.upsert', () => {
      console.log('✉️ Got chats', store.chats.all())
   })

   sock.ev.on('contacts.upsert', () => {
      console.log('👥 Got contacts', Object.values(store.contacts))
   })

   store.readFromFile(storePath)

   setInterval(() => {
      store.writeToFile(storePath)
   }, 180000)
}

connectToWhatsApp()
```

---

### 🪪 WhatsApp IDs Explain

`id` is the WhatsApp ID (also referred to as `jid` or `lid`) of the person or group you're messaging.
- Format: `[country code][phone number]@s.whatsapp.net`
   - Individual: `19999999999@s.whatsapp.net` or `12699999999@lid`
   - Group: `123456789-123345@g.us`
- Meta AI: `11111111111@bot`
- Broadcast lists: `[timestamp]@broadcast`
- Stories: `status@broadcast`

---

### ✉️ Sending Messages

#### 🔠 Text

```javascript
// --- Regular text
sock.sendMessage(jid, {
   text: '👋🏻 Hello'
}, {
   quoted: message
})

// --- With link preview
const urlA = 'https://www.npmjs.com/package/@lordmega/baileys'

sock.sendMessage(jid, {
   text: urlA + ' 👆🏻 Check it out!',
   linkPreview: {
      'matched-text': urlA,
      title: '🌱 @lordmega/baileys',
      description: 'Underrated Baileys Fork',
      previewType: 0,
      jpegThumbnail: fs.readFileSync('./path/to/image.jpg')
   }
})

// --- Large link preview with favicon
import { prepareWAMessageMedia } from '@lordmega/baileys'

const urlB = 'https://www.npmjs.com/package/@lordmega/baileys#readme'

const { imageMessage: image } = await prepareWAMessageMedia({
   image: { url: './path/to/image.jpg' }
}, {
   upload: sock.waUploadToServer,
   mediaTypeOverride: 'thumbnail-link'
})

image.height = 720
image.width = 480

sock.sendMessage(jid, {
   text: urlB + ' 👆🏻 Check it out!',
   linkPreview: {
      'matched-text': urlB,
      title: '🌱 @lordmega/baileys',
      description: 'Underrated Baileys Fork',
      previewType: 0,
      jpegThumbnail: fs.readFileSync('./path/to/image.jpg'),
      highQualityThumbnail: image,
      linkPreviewMetadata: {
         linkMediaDuration: 0,
         socialMediaPostType: 1,
      }
   },
   favicon: { url: './path/to/tiny-image.ico' }
})
```

#### 🔔 Mention

```javascript
// --- Specific mention
sock.sendMessage(jid, {
   text: '👋🏻 Hello @628123456789',
   mentions: ['628123456789@s.whatsapp.net']
}, {
   quoted: message
})

// --- Mention all
sock.sendMessage(jid, {
   text: '👋🏻 Hello @all',
   mentionAll: true
}, {
   quoted: message
})
```

#### 😁 Reaction

```javascript
sock.sendMessage(jid, {
   react: {
      key: message.key,
      text: '✨'
   }
})
```

#### 📌 Pin Message

```javascript
sock.sendMessage(jid, {
   pin: message.key,
   time: 86400, // 86400 (1d), 604800 (7d), 2592000 (30d)
   type: 1 // 2 to unpin
})
```

#### 🔖 Keep Chat

> [!NOTE]
> Only works in chats or groups with disappearing messages enabled.

```javascript
sock.sendMessage(jid, {
   keep: message.key,
   type: 1 // 2 to remove
})
```

#### ➡️ Forward Message

```javascript
sock.sendMessage(jid, {
   forward: message,
   force: true // Optional
})
```

#### 👤 Contact

```javascript
const vcard = 'BEGIN:VCARD\n'
            + 'VERSION:3.0\n'
            + 'FN:John Doe\n'
            + 'ORG:Example;\n'
            + 'TEL;type=CELL;type=VOICE;waid=628123456789:+62 8123 4567 89\n'
            + 'END:VCARD'

sock.sendMessage(jid, {
   contacts: {
      displayName: 'John Doe',
      contacts: [{ vcard }]
   }
}, {
   quoted: message
})
```

#### 📍 Location

```javascript
sock.sendMessage(jid, {
   location: {
      degreesLatitude: 24.121231,
      degreesLongitude: 55.1121221,
      name: '👋🏻 I am here'
   }
}, {
   quoted: message
})
```

#### 🗓️ Event

```javascript
sock.sendMessage(jid, {
   event: {
      name: '🎶 Meet & Mingle Party',
      description: 'A casual gathering to connect and build new relationships.',
      call: 'audio', // or "video", optional
      startDate: new Date(Date.now() + 3600000),
      endDate: new Date(Date.now() + 28800000),
      isCancelled: false,
      isScheduleCall: false,
      extraGuestsAllowed: false,
      location: {
         name: 'Jakarta',
         degreesLatitude: -6.2,
         degreesLongitude: 106.8
      }
   }
}, {
   quoted: message
})
```

#### 👥 Group Invite

```javascript
const inviteCode = groupUrl
   .split('chat.whatsapp.com/')[1]
   ?.split('?')[0]

sock.sendMessage(jid, {
   groupInvite: {
      inviteCode,
      inviteExpiration: Date.now() + 86400000,
      text: '👋🏻 You are invited to join our group.',
      jid: '1201111111111@g.us',
      subject: 'Group Name',
   }
}, {
   quoted: message
})
```

#### 🛍️ Product

```javascript
import { randomUUID } from 'crypto'

sock.sendMessage(jid, {
   image: { url: './path/to/image.jpg' },
   body: '👋🏻 Check this out!',
   footer: 'MegaBot',
   product: {
      currencyCode: 'IDR',
      description: '🛍️ Great product!',
      priceAmount1000: 70_000_000,
      productId: randomUUID(),
      productImageCount: 1,
      salePriceAmount1000: 65_000_000,
      signedUrl: 'https://example.com',
      title: '📦 Product Name',
      url: 'https://example.com'
   },
   businessOwnerJid: '0@s.whatsapp.net'
})
```

#### 📊 Poll

```javascript
// --- Standard poll
sock.sendMessage(jid, {
   poll: {
      name: '🔥 Quick vote',
      values: ['Yes', 'No'],
      selectableCount: 1,
      toAnnouncementGroup: false,
      endDate: new Date(Date.now() + 28800000),
      hideVoter: false,
      canAddOption: false
   }
}, {
   quoted: message
})

// --- Quiz (newsletters only)
sock.sendMessage('1211111111111@newsletter', {
   poll: {
      name: '🔥 Quiz',
      values: ['Yes', 'No'],
      correctAnswer: 'Yes',
      pollType: 1
   }
})

// --- Poll result
sock.sendMessage(jid, {
   pollResult: {
      name: '📝 Poll Result',
      votes: [{
         name: 'Nice',
         voteCount: 10
      }, {
         name: 'Nah',
         voteCount: 2
      }],
      pollType: 0
   }
})

// --- Poll update
sock.sendMessage(jid, {
   pollUpdate: {
      metadata: {},
      key: message.key,
      vote: {
         enclv: /* <Buffer> */,
         encPayload: /* <Buffer> */
      }
   }
})
```

#### 💭 Button Response

```javascript
// --- buttonsResponseMessage
sock.sendMessage(jid, {
   type: 'plain',
   buttonReply: {
      id: '#Menu',
      displayText: '✨ Menu'
   }
}, { quoted: message })

// --- interactiveResponseMessage
sock.sendMessage(jid, {
   flowReply: {
      format: 0,
      text: '💭 Response',
      name: 'menu_options',
      paramsJson: JSON.stringify({
         id: '#Menu',
         description: '✨ Menu'
      })
   }
}, { quoted: message })

// --- listResponseMessage
sock.sendMessage(jid, {
   listReply: {
      title: '📄 See More',
      description: '✨ Menu',
      id: '#Menu'
   }
}, { quoted: message })

// --- templateButtonReplyMessage
sock.sendMessage(jid, {
   type: 'template',
   buttonReply: {
      id: '#Menu',
      displayText: '✨ Menu',
      index: 1
   }
}, { quoted: message })
```

#### ✨ Rich Response

> [!NOTE]
> `richResponse[]` maps to `submessages[]` inside `richResponseMessage`.

```javascript
sock.sendMessage(jid, {
   disclaimerText: 'RAW submessages structure example',
   richResponse: [{
      text: 'Example Usage',
   }, {
      language: 'javascript',
      code: [{
         highlightType: 0,
         codeContent: 'console.log("Hello, World!")'
      }]
   }, {
      text: 'Pretty simple, right?\n'
   }, {
      text: 'Runtime Comparison',
   }, {
      title: 'Runtime Comparison',
      table: [{
         isHeading: true,
         items: ['', 'Node.js', 'Bun', 'Deno']
      }, {
         isHeading: false,
         items: ['Engine', 'V8 (C++)', 'JavaScriptCore (C++)', 'V8 (C++)']
      }, {
         isHeading: false,
         items: ['Performance', '4/5', '5/5', '4/5']
      }]
   }, {
      text: 'Does this help clarify the differences?'
   }]
})
```

> [!TIP]
> Use `tokenizeCode` for syntax highlighting:

```javascript
import { tokenizeCode } from '@lordmega/baileys'

const language = 'javascript'
const code = 'console.log("Hello, World!")'

sock.sendMessage(jid, {
   disclaimerText: 'Tokenized Code Block',
   richResponse: [{
      text: 'Example',
   }, {
      language,
      code: tokenizeCode(code, language)
   }, {
      text: 'Clean and simple.'
   }]
})
```

> 💡 Supported languages: `css`, `html`, `javascript`, `typescript`, `python`, `golang`, `rust`, `c`, `c#`, `c++`, `bash`, `bat`, `powershell`

#### 🧾 Message with Code Block

```javascript
sock.sendMessage(jid, {
   disclaimerText: 'Code Block',
   headerText: '## Example Usage',
   contentText: '---',
   code: 'console.log("Hello, World!")',
   language: 'javascript',
   footerText: 'Pretty simple, right?'
})
```

#### 🌏 Message with Inline Entities

```javascript
sock.sendMessage(jid, {
   disclaimerText: 'Inline Entities',
   headerText: '## Check Out!',
   contentText: '---',
   links: [{
      text: '1. Google',
      title: 'Popular Search Engine',
      url: 'https://www.google.com/'
   }, {
      text: '2. YouTube',
      title: 'Popular Streaming Platform',
      url: 'https://www.youtube.com/'
   }],
   footerText: '---'
})
```

#### 📋 Message with Table

```javascript
sock.sendMessage(jid, {
   disclaimerText: 'Table',
   headerText: '## Runtime Comparison',
   contentText: '---',
   title: 'Node.js vs Bun vs Deno',
   table: [
      ['', 'Node.js', 'Bun', 'Deno'],
      ['Engine', 'V8 (C++)', 'JavaScriptCore (C++)', 'V8 (C++)'],
      ['Performance', '4/5', '5/5', '4/5']
   ],
   noHeading: false,
   footerText: 'Does this help clarify things?'
})
```

#### 🎞️ Status Mention

```javascript
sock.sendMessage([jidA, jidB, jidC], {
   text: 'Hello! 👋🏻'
})
```

---

### 📁 Sending Media Messages

> [!NOTE]
> Media can be passed as a `Buffer`, `{ stream: Readable }`, or `{ url: string }` (local path or HTTP/HTTPS URL).

#### 🖼️ Image

```javascript
sock.sendMessage(jid, {
   image: { url: './path/to/image.jpg' },
   caption: '🔥 Check this out'
}, { quoted: message })
```

#### 🎥 Video

```javascript
sock.sendMessage(jid, {
   video: { url: './path/to/video.mp4' },
   gifPlayback: false,
   ptv: false,
   caption: '🔥 Check this out'
}, { quoted: message })
```

#### 📃 Sticker

```javascript
sock.sendMessage(jid, {
   sticker: { url: './path/to/sticker.webp' }
}, { quoted: message })
```

#### 💽 Audio

```javascript
sock.sendMessage(jid, {
   audio: { url: './path/to/audio.mp3' },
   ptt: false // true for voice note
}, { quoted: message })
```

#### 🗂️ Document

```javascript
sock.sendMessage(jid, {
   document: { url: './path/to/document.pdf' },
   mimetype: 'application/pdf',
   caption: '✨ Document'
}, { quoted: message })
```

#### 🖼️ Album (Image & Video)

```javascript
sock.sendMessage(jid, {
   album: [{
      image: { url: './path/to/image.jpg' },
      caption: '1st image'
   }, {
      video: { url: './path/to/video.mp4' },
      caption: '1st video'
   }, {
      image: { url: './path/to/image.jpg' },
      caption: '2nd image'
   }, {
      video: { url: './path/to/video.mp4' },
      caption: '2nd video'
   }]
}, { quoted: message })
```

#### 📦 Sticker Pack

> [!IMPORTANT]
> Without `sharp` or `@napi-rs/image` installed, all sticker files must already be in WebP format.

```javascript
sock.sendMessage(jid, {
   cover: { url: './path/to/image.webp' },
   stickers: [{
      data: { url: './path/to/image.webp' }
   }, {
      data: { url: './path/to/image.webp' }
   }],
   name: '📦 My Sticker Pack',
   publisher: 'MegaBot',
   description: 'Custom sticker pack'
}, { quoted: message })
```

---

### 👁️ Reveal View-Once

Download a view-once message and resend it as normal media. Works for image, video, audio, document, and sticker. Downloads and re-uploads so it stays valid even after the original was opened.

```javascript
sock.ev.on('messages.upsert', async ({ messages }) => {
  for (const m of messages) {
    const vo = m.message?.viewOnceMessage
      || m.message?.viewOnceMessageV2
      || m.message?.viewOnceMessageV2Extension
    if (vo) {
      await sock.rvo(m)           // resend to the original chat
      // await sock.rvo(m, jid)   // or to a specific jid
    }
  }
})
```

---

### 👉🏻 Sending Interactive Messages

#### 🔘 Buttons

```javascript
// --- Basic buttons
sock.sendMessage(jid, {
   text: '👆🏻 Buttons!',
   footer: 'MegaBot',
   buttons: [{
      text: '👋🏻 Sign Up',
      id: '#SignUp'
   }]
}, { quoted: message })

// --- Buttons with media and native flow
sock.sendMessage(jid, {
   image: { url: './path/to/image.jpg' },
   caption: '👆🏻 Buttons with Native Flow!',
   footer: 'MegaBot',
   buttons: [{
      text: '👋🏻 Rating',
      id: '#Rating'
   }, {
      text: '📋 Select',
      sections: [{
         title: '✨ Section 1',
         rows: [{
            header: '',
            title: '💭 Secret Ingredient',
            description: '',
            id: '#SecretIngredient'
         }]
      }]
   }]
}, { quoted: message })
```

#### 📋 List

> [!NOTE]
> Only works in private chats (`@s.whatsapp.net`).

```javascript
sock.sendMessage(jid, {
   text: '📋 Pick an option',
   footer: 'MegaBot',
   buttonText: '📋 Select',
   title: '👋🏻 Hello',
   sections: [{
      title: '🚀 Menu 1',
      rows: [{
         title: '✨ AI',
         description: '',
         rowId: '#AI'
      }]
   }, {
      title: '🌱 Menu 2',
      rows: [{
         title: '🔍 Search',
         description: '',
         rowId: '#Search'
      }]
   }]
}, { quoted: message })
```

#### 🗄️ Interactive

```javascript
// --- Native flow
sock.sendMessage(jid, {
   image: { url: './path/to/image.jpg' },
   caption: '🗄️ Interactive!',
   footer: 'MegaBot',
   optionText: '👉🏻 Select Options',
   optionTitle: '📄 Options',
   offerText: '🏷️ Latest Deal!',
   offerCode: 'MEGA2024',
   offerUrl: 'https://example.com',
   offerExpiration: Date.now() + 3_600_000,
   nativeFlow: [{
      text: '👋🏻 Greeting',
      id: '#Greeting',
      icon: 'review'
   }, {
      text: '📞 Call',
      call: '628123456789'
   }, {
      text: '📋 Copy',
      copy: 'some-text'
   }, {
      text: '🌐 Visit',
      url: 'https://example.com',
      useWebview: true
   }, {
      text: '📋 Select',
      sections: [{
         title: '✨ Section 1',
         rows: [{
            header: '',
            title: '🏷️ Option A',
            description: '',
            id: '#OptionA'
         }]
      }],
      icon: 'default'
   }],
   interactiveAsTemplate: false // Optional, wrap into templateMessage
}, { quoted: message })

// --- Carousel with native flow
sock.sendMessage(jid, {
   text: '🗂️ Carousel!',
   footer: 'MegaBot',
   cards: [{
      image: { url: './path/to/image.jpg' },
      caption: '🖼️ Slide 1',
      footer: '🏷️ Tag',
      nativeFlow: [{
         text: '🌐 Visit',
         url: 'https://example.com',
         useWebview: true
      }]
   }, {
      image: { url: './path/to/image.jpg' },
      caption: '🖼️ Slide 2',
      footer: '🏷️ Tag',
      nativeFlow: [{
         text: '🌐 Visit',
         url: 'https://example.com'
      }]
   }]
}, { quoted: message })

// --- Native flow with audio footer
sock.sendMessage(jid, {
   text: '🔈 Audio in footer!',
   audioFooter: { url: './path/to/audio.mp3' },
   nativeFlow: [{
      text: '👍🏻 Next',
      id: '#Next',
      icon: 'review'
   }, {
      text: '👎🏻 Skip',
      id: '#Skip',
      icon: 'default'
   }]
}, { quoted: message })
```

#### 🫙 Hydrated Template

```javascript
sock.sendMessage(jid, {
   title: '👋🏻 Hello',
   image: { url: './path/to/image.jpg' },
   caption: '🫙 Template!',
   footer: 'MegaBot',
   templateButtons: [{
      text: '👉🏻 Tap Here',
      id: '#Order'
   }, {
      text: '🌐 Visit',
      url: 'https://example.com'
   }, {
      text: '📞 Call',
      call: '628123456789'
   }]
}, { quoted: message })
```

---

### 💳 Sending Payment Messages

#### ➕ Invite Payment

```javascript
sock.sendMessage(jid, {
   paymentInviteServiceType: 3 // 1, 2, or 3
})
```

#### 🧾 Invoice

> [!NOTE]
> Invoice messages are not fully supported yet.

```javascript
sock.sendMessage(jid, {
   image: { url: './path/to/image.jpg' },
   invoiceNote: '🏷️ Invoice'
})
```

#### 🛍️ Order

```javascript
sock.sendMessage(jid, {
   orderText: '🛍️ Your Order',
   thumbnail: fs.readFileSync('./path/to/image.jpg') // Must be a Buffer
}, { quoted: message })
```

#### 💳 Request Payment

```javascript
sock.sendMessage(jid, {
   text: '💳 Payment Request',
   requestPaymentFrom: '0@s.whatsapp.net'
})
```

---

### 👁️ Other Message Options

#### 🤖 AI Icon

> [!NOTE]
> Only works in private chats (`@s.whatsapp.net`).

```javascript
sock.sendMessage(jid, {
   image: { url: './path/to/image.jpg' },
   caption: '🤖 AI-tagged message',
   ai: true
}, { quoted: message })
```

#### 🕒 Ephemeral

```javascript
sock.sendMessage(jid, {
   image: { url: './path/to/image.jpg' },
   caption: '👁️ Ephemeral',
   ephemeral: true
})
```

#### 📰 External Ad Reply

```javascript
sock.sendMessage(jid, {
   text: '📰 Ad Reply',
   externalAdReply: {
      title: '📝 Did you know?',
      body: '❓ Interesting fact',
      thumbnail: fs.readFileSync('./path/to/image.jpg'),
      largeThumbnail: false,
      url: 'https://example.com'
   }
}, { quoted: message })
```

#### 🧑‍🧑‍🧒 Group Status

> [!NOTE]
> Only works in group chats (`@g.us`).

```javascript
sock.sendMessage(jid, {
   image: { url: './path/to/image.jpg' },
   caption: '👥 Group Status',
   groupStatus: true
})
```

#### 🐱 Lottie Sticker

```javascript
sock.sendMessage(jid, {
   sticker: { url: './path/to/sticker.webp' },
   isLottie: true
})
```

#### 🧩 Raw

```javascript
sock.sendMessage(jid, {
   extendedTextMessage: {
      text: '📃 Manually constructed proto message',
      contextInfo: {
         externalAdReply: {
            title: 'MegaBot',
            thumbnail: fs.readFileSync('./path/to/image.jpg'),
            sourceApp: 'whatsapp',
            showAdAttribution: true,
            mediaType: 1
         }
      }
   },
   raw: true
}, { quoted: message })
```

#### 🏷️ Secure Meta Service Label

```javascript
sock.sendMessage(jid, {
   text: '🏷️ Labeled message',
   secureMetaServiceLabel: true
})
```

#### 📑 Spoiler

```javascript
sock.sendMessage(jid, {
   image: { url: './path/to/image.jpg' },
   caption: '❔ Spoiler',
   spoiler: true
})
```

#### 👁️ View Once

```javascript
sock.sendMessage(jid, {
   image: { url: './path/to/image.jpg' },
   caption: '👁️ View Once',
   viewOnce: true
})
```

#### 👁️ View Once V2

```javascript
sock.sendMessage(jid, {
   image: { url: './path/to/image.jpg' },
   caption: '👁️ View Once V2',
   viewOnceV2: true
})
```

#### 👁️ View Once V2 Extension

```javascript
sock.sendMessage(jid, {
   image: { url: './path/to/image.jpg' },
   caption: '👁️ View Once V2 Extension',
   viewOnceV2Extension: true
})
```

#### 🔑 Caller-Supplied messageSecret

Pass your own 32-byte `messageSecret` on any message type:

```javascript
import { randomBytes } from 'crypto'

await sock.sendMessage(jid, { text: 'hi' }, { messageSecret: randomBytes(32) })
```

---

### ♻️ Modify Messages

#### 🗑️ Delete Messages

```javascript
sock.sendMessage(jid, {
   delete: message.key
})
```

#### ✏️ Edit Messages

```javascript
// --- Edit text
sock.sendMessage(jid, {
   text: '✨ Corrected message',
   edit: message.key
})

// --- Edit media caption
sock.sendMessage(jid, {
   caption: '✨ Updated caption',
   edit: message.key
})
```

> [!NOTE]
> Encrypted E2EE message edits (May 2026+) are automatically decrypted — edited messages arrive via the normal `protocolMessage.editedMessage` path.

---

### 🧰 Additional Contents

#### 🏷️ Find User ID (JID|PN/LID)

> [!NOTE]
> Numbers only — no `+`, `()`, or `-`. Must include country code.

```javascript
const ids = await sock.findUserId('6281111111111@s.whatsapp.net')
console.log('🏷️ User ID:', ids)

// Output:
// { phoneNumber: '6281111111111@s.whatsapp.net', lid: '43411111111111@lid' }
// On failure:
// { phoneNumber: '6281111111111@s.whatsapp.net', lid: undefined }
```

#### 🔑 Request Custom Pairing Code

```javascript
await sock.requestPairingCode('6281111111111', 'MYCODE')
console.log('🔗 Pairing code: MYCODE')
```

#### 🖼️ Image Processing

```javascript
import { getImageProcessingLibrary } from '@lordmega/baileys'
import { readFile } from 'fs/promises'

const lib = await getImageProcessingLibrary()
const input = './path/to/image.jpg'
const width = 512
let output

if (lib.sharp?.default) {
   output = await lib.sharp.default(input)
      .resize(width)
      .jpeg({ quality: 80 })
      .toBuffer()
}
else if (lib.image?.Transformer) {
   const buf = Buffer.isBuffer(input) ? input : await readFile(input)
   output = await new lib.image.Transformer(buf)
      .resize(width, undefined, 0)
      .jpeg(50)
}
else if (lib.jimp?.Jimp) {
   output = await (await lib.jimp.Jimp.read(input))
      .resize({ w: width, mode: lib.jimp.ResizeStrategy.BILINEAR })
      .getBuffer('image/jpeg', { quality: 50 })
}
else {
   throw new Error('No image processing library available')
}
```

#### 📣 Newsletter Management

```javascript
sock.newsletterCreate('Name', 'Description')
const metadata = sock.newsletterMetadata('1231111111111@newsletter')
const subscribers = await sock.newsletterSubscribers('1231111111111@newsletter')
sock.newsletterFollow('1231111111111@newsletter')
sock.newsletterUnfollow('1231111111111@newsletter')
sock.newsletterMute('1231111111111@newsletter')
sock.newsletterUnmute('1231111111111@newsletter')
sock.newsletterDemote('1231111111111@newsletter', '628...@s.whatsapp.net')
sock.newsletterChangeOwner('1231111111111@newsletter', '628...@s.whatsapp.net')
sock.newsletterUpdate('1231111111111@newsletter', { name: 'New Name' })
sock.newsletterUpdateName('1231111111111@newsletter', 'New Name')
sock.newsletterUpdateDescription('1231111111111@newsletter', 'New description')
sock.newsletterUpdatePicture('1231111111111@newsletter', { url: 'path/to/image.jpg' })
sock.newsletterRemovePicture('1231111111111@newsletter')
sock.newsletterReactMessage('1231111111111@newsletter', '100', '💛')
const count = await sock.newsletterAdminCount('1231111111111@newsletter')
const newsletters = await sock.newsletterSubscribed()
const messages = sock.newsletterFetchMessages('jid', '1231111111111@newsletter', 50, 0, 0)
sock.newsletterDelete('1231111111111@newsletter')
```

#### 👥 Group Management

```javascript
const group = sock.groupCreate('Group Name', ['628...@s.whatsapp.net'])
const metadata = await sock.groupMetadata(jid)
const inviteCode = await sock.groupInviteCode(jid)
sock.groupRevokeInvite(jid)
sock.groupAcceptInvite(inviteCode)
sock.groupLeave(jid)
sock.groupParticipantsUpdate(jid, ['628...@s.whatsapp.net'], 'add')
sock.groupParticipantsUpdate(jid, ['628...@s.whatsapp.net'], 'remove')
sock.groupParticipantsUpdate(jid, ['628...@s.whatsapp.net'], 'promote')
sock.groupParticipantsUpdate(jid, ['628...@s.whatsapp.net'], 'demote')
sock.groupRequestParticipantsUpdate(jid, ['628...@s.whatsapp.net'], 'approve')
sock.groupUpdateSubject(jid, 'New Name')
sock.groupUpdateDescription(jid, 'New description')
sock.updateProfilePicture(jid, { url: 'path/to/image.jpg' })
sock.removeProfilePicture(jid)
sock.groupSettingUpdate(jid, 'announcement')    // admin-only chat
sock.groupSettingUpdate(jid, 'not_announcement') // open chat
sock.groupSettingUpdate(jid, 'locked')           // admin-only edits
sock.groupSettingUpdate(jid, 'unlocked')         // open edits
sock.groupMemberAddMode(jid, 'admin_add')
sock.groupMemberAddMode(jid, 'all_member_add')
sock.groupToggleEphemeral(jid, 86400)
sock.groupToggleEphemeral(jid, 0) // disable
sock.groupJoinApprovalMode(jid, 'on')
sock.groupJoinApprovalMode(jid, 'off')
const groups = await sock.groupFetchAllParticipating()
const requests = await sock.groupRequestParticipantsList(jid)
const groupInfo = await sock.groupGetInviteInfo('ABC123456789')
sock.updateMemberLabel(jid, 'label')
```

#### 👥 Community Management

```javascript
const community = await sock.communityCreate('Name', 'Description')
const group = await sock.communityCreateGroup('Announcements', ['628...@s.whatsapp.net'], communityJid)
sock.communityLinkGroup(groupJid, communityJid)
sock.communityUnlinkGroup(groupJid, communityJid)
const metadata = await sock.communityMetadata(jid)
const inviteCode = await sock.communityInviteCode(jid)
sock.communityRevokeInvite(jid)
sock.communityAcceptInvite(inviteCode)
sock.communityLeave(jid)
sock.communityRequestParticipantsUpdate(jid, ['628...@s.whatsapp.net'], 'approve')
sock.communityUpdateSubject(jid, 'New Name')
sock.communityUpdateDescription(jid, 'New description')
sock.communitySettingUpdate(jid, 'announcement')
sock.communitySettingUpdate(jid, 'locked')
sock.communityMemberAddMode(jid, 'admin_add')
sock.communityToggleEphemeral(jid, 86400)
sock.communityJoinApprovalMode(jid, 'on')
const communities = await sock.communityFetchAllParticipating()
const linked = await sock.communityFetchLinkedGroups(jid)
const requests = await sock.communityRequestParticipantsList(jid)
const info = await sock.communityGetInviteInfo('ABC123456789')
```

#### 👤 Profile Management

```javascript
const url = await sock.profilePictureUrl(jid, 'image')
sock.updateProfilePicture(jid, buffer)
sock.removeProfilePicture(jid)
sock.updateProfileName('My Name')
sock.updateProfileStatus('Available')
sock.sendPresenceUpdate('available', jid)
sock.presenceSubscribe(jid)
sock.readMessages([message.key])
sock.sendReceipt(jid, participant, [messageId], 'read')
sock.updateBlockStatus(jid, 'block')
sock.updateBlockStatus(jid, 'unblock')
const blocked = await sock.fetchBlocklist()
sock.chatModify({ archive: true, lastMessageOrig: message, lastMessage: message }, jid)
sock.star(jid, [{ id: messageId, fromMe: true }], true)
sock.addOrEditContact(jid, { displayName: 'Name' })
sock.removeContact(jid)
sock.addChatLabel(jid, labelId)
sock.removeChatLabel(jid, labelId)
sock.addMessageLabel(jid, messageId, labelId)
sock.resyncAppState(['regular', 'critical_block'], true)
const profile = await sock.getBusinessProfile(jid)
```

#### 🛒 Business Management

```javascript
const product = await sock.productCreate({
   name: 'Product Name',
   description: 'Description',
   price: 100000,
   currency: 'IDR',
   originCountryCode: 'ID',
   images: [bufferImage, { url: './path/to/image.jpg' }]
})

await sock.productUpdate(productId, {
   name: 'Updated Name',
   price: 75000,
   currency: 'IDR',
   images: [{ url: './path/to/image.jpg' }]
})

sock.productDelete([productId])

const { products, nextPageCursor } = await sock.getCatalog({
   jid: '628...@s.whatsapp.net',
   limit: 10
})

const collections = await sock.getCollections('628...@s.whatsapp.net', 10)
const order = await sock.getOrderDetails(orderId, tokenBase64)

await sock.updateBusinessProfile({
   address: 'Jakarta, Indonesia',
   description: 'Official Store',
   websites: ['https://example.com'],
   email: 'contact@example.com',
   hours: {
      timezone: 'Asia/Jakarta',
      days: [{ day: 'mon', mode: 'open_24h' }]
   }
})

sock.updateCoverPhoto({ url: './path/to/image.jpg' })
sock.removeCoverPhoto(coverId)
sock.addOrEditQuickReply({ shortcut: 'hello', message: 'Hello!' })
sock.removeQuickReply(timestamp)
```

#### 🔐 Privacy Management

```javascript
sock.updateLastSeenPrivacy('all' | 'contacts' | 'contact_blacklist' | 'nobody')
sock.updateOnlinePrivacy('all' | 'match_last_seen')
sock.updateProfilePicturePrivacy('contacts')
sock.updateStatusPrivacy('contacts')
sock.updateReadReceiptsPrivacy('all' | 'none')
sock.updateGroupsAddPrivacy('all' | 'contacts')
sock.updateMessagesPrivacy('all' | 'contacts' | 'nobody')
sock.updateCallPrivacy('everyone')
sock.updateDefaultDisappearingMode(86400)
sock.updateDisableLinkPreviewsPrivacy(true)
```

#### 📡 Events

```javascript
sock.ev.on('connection.update', (update) => {})
sock.ev.on('creds.update', (update) => {})
sock.ev.on('messaging-history.set', (update) => {})
sock.ev.on('messaging-history.status', (update) => {})
sock.ev.on('chats.upsert', (update) => {})
sock.ev.on('chats.update', (update) => {})
sock.ev.on('chats.delete', (update) => {})
sock.ev.on('chats.lock', (update) => {})
sock.ev.on('lid-mapping.update', (update) => {})
sock.ev.on('presence.update', (update) => {})
sock.ev.on('contacts.upsert', (update) => {})
sock.ev.on('contacts.update', (update) => {})
sock.ev.on('messages.delete', (update) => {})
sock.ev.on('messages.update', (update) => {})
sock.ev.on('messages.media-update', (update) => {})
sock.ev.on('messages.upsert', (update) => {})
sock.ev.on('messages.reaction', (update) => {})
sock.ev.on('message-receipt.update', (update) => {})
sock.ev.on('groups.upsert', (update) => {})
sock.ev.on('groups.update', (update) => {})
sock.ev.on('group-participants.update', (update) => {})
sock.ev.on('group.join-request', (update) => {})
sock.ev.on('group.member-tag.update', (update) => {})
sock.ev.on('blocklist.set', (update) => {})
sock.ev.on('blocklist.update', (update) => {})
sock.ev.on('call', (update) => {})
sock.ev.on('labels.edit', (update) => {})
sock.ev.on('labels.association', (update) => {})
sock.ev.on('newsletter.reaction', (update) => {})
sock.ev.on('newsletter.view', (update) => {})
sock.ev.on('newsletter-participants.update', (update) => {})
sock.ev.on('newsletter-settings.update', (update) => {})
sock.ev.on('settings.update', (update) => {})
```

---

### 🚀 Try the Bot

A lightweight, modular WhatsApp bot built on this library — includes group management, moderation, quiz games, and utility tools.

👉🏻 [MegaBot MD](https://github.com/LORDMEGA-MD/MegaBot)

---

### 📦 Fork Base

Based on [WhiskeySockets/Baileys](https://github.com/WhiskeySockets/Baileys)
