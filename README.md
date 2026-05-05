# Sharencrypt - Secure P2P File Sharing

A secure, peer-to-peer file sharing web app built with WebRTC. Files are transferred directly between browsers — no server, no storage, no tracking.

---

## Features

- **End-to-End Encrypted** - AES-GCM 256-bit encryption on every transfer
- **True P2P** - Direct browser-to-browser connection via WebRTC
- **No File Size Limits** - Share large files without restrictions
- **Folder Support** - Folders are auto-zipped before transfer using Web Workers
- **QR Code Pairing** - Scan to connect instantly on mobile
- **Clipboard Paste** - Ctrl+V to send screenshots directly
- **Responsive UI** - Built with React 18, Tailwind CSS, and Framer Motion

---

## Tech Stack

- **Frontend**: React 18, TypeScript, Tailwind CSS, Framer Motion
- **P2P**: WebRTC, PeerJS
- **Encryption**: AES-GCM via Web Crypto API
- **Background Processing**: Web Workers (encryption + zipping)
- **Build Tool**: Vite

---

## Getting Started

### Prerequisites
- Node.js 14+
- npm or yarn

### Installation

```bash
# Clone the repo
git clone https://github.com/rithikareddy714-bit/p2p-file-share.git
cd p2p-file-share

# Install dependencies
npm install

# Start the dev server
npm run dev
```

Open `http://localhost:5173` in your browser.

---

## How It Works

1. User A opens the app and gets a unique Peer ID
2. User B connects using that ID (or scans the QR code)
3. A direct WebRTC connection is established
4. Files are encrypted and transferred directly — no server involved

---

## Project Structure

```
src/
├── components/       # UI components
├── hooks/            # usePeerConnection (core P2P logic)
├── services/         # Connection & transfer managers
├── workers/          # Background encryption & zipping
└── utils/            # Encryption helpers
```

---

## License

AGPL v3.0 — see [LICENSE](./LICENSE) for details.

---

Made by Rithika Reddy
