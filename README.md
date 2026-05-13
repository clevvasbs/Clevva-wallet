# Clevva - Base Wallet

Secure 4-digit passcode wallet on Base.

### Stack
- Next.js 14 App Router
- wagmi + viem for Base chain  
- Tailwind CSS
- Cloudflare Pages
- Resend for email alerts

### Local Dev
Copy `.env.example` to `.env.local` and add your keys.

```
npm install
npm run dev
```

### Deploy
Push to `main` → Auto-deploys to Cloudflare Pages  
Live: https://clevva.sbs

### Security
Passcode gate is client-side UX only. Add wallet signature auth for production.

```
NEXT_PUBLIC_PASSCODE=1234
RESEND_API_KEY=your-resend-api-key
NEXT_PUBLIC_WALLETCONNECT_PROJECT_ID=your-wc-project-id
NEXT_PUBLIC_BASE_RPC=https://mainnet.base.org
NEXT_PUBLIC_APP_URL=https://clevva.sbs
```
