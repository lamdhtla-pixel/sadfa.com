# CryptoPulse - Worldwide Cryptocurrency Rewards & Advertising Platform

A full-featured cryptocurrency rewards and advertising web application designed with the same structure, services, layout, and user experience as industry-leading platforms such as Cointiply, FaucetPay, and CoinPayU.

---

## 🌍 Worldwide Access & Registration
- **200+ Countries Supported**: Users from any sovereign nation or territory worldwide can register, complete tasks, claim rewards, deposit, and withdraw without geographic restrictions or IP blocks.
- **Global Country Selector**: Full country selection with national flags during registration and in profile settings.
- **Multi-Currency Display**: Real-time conversion across 14 fiat currencies (USD, EUR, GBP, JPY, CAD, AUD, BRL, NGN, INR, RUB, VND, IDR, TRY, PHP).
- **Global Geo-Targeting for Advertisers**: Target Worldwide, North America, Europe, Asia-Pacific, Latin America, or Africa & Middle East.

---

## 📱 Cross-Device Compatibility (Android, iPhone & Desktop)
- **iPhone / iOS Optimization**:
  - Safe-area insets support (`env(safe-area-inset-top)`, `env(safe-area-inset-bottom)`) for iPhone notch, Dynamic Island, and Home Indicator bar.
  - Apple Web App meta tags (`apple-mobile-web-app-capable`, `apple-mobile-web-app-status-bar-style`).
  - Font-size 16px safeguard on inputs to eliminate iOS Safari automatic zoom-in on focus.
  - Momentum touch scrolling (`-webkit-overflow-scrolling: touch`).
- **Android Optimization**:
  - `theme-color` meta tag for seamless Chrome status bar and navigation bar integration.
  - High-precision touch targets (min 44px tap targets adhering to Material Design).
  - Web App capable manifest & viewport fit covers.
- **Off-Canvas Mobile Drawer**:
  - Smooth slide-in navigation sidebar on mobile phones with tap-to-dismiss background overlay.
  - Thumb-friendly Mobile Bottom Navigation Bar (Dashboard, Faucet, PTC, Wallet, Menu).
- **Desktop Computers**:
  - Full widescreen responsive layouts, keyboard-friendly navigation, sticky header, and multi-column dashboards.

---

## 🚀 How to Run the Website

### Method 1: Local Server (PowerShell)
Open PowerShell in the project directory and run:
```powershell
.\server.ps1
```
The server will start at `http://localhost:3000` and automatically launch your default browser.

### Method 2: Direct File Open
You can directly open `index.html` in any modern web browser (Google Chrome, Microsoft Edge, Mozilla Firefox, Brave, Safari). All features, audio synthesizers, confetti animations, and state persistence via `localStorage` work out of the box with zero external dependencies.

---

## 👥 Demo Profiles & Role Switcher
A quick role-switcher is included directly in the top navigation bar:
- **Alex_Crypto (Earner)**: Level 4 user, 2,850 Coins ($2.85 USD), 4-day active loyalty streak, wallet addresses preset.
- **CryptoNewbie (New Earner)**: Level 1 user, 120 Coins ($0.12 USD), zero claims today.
- **AlphaMedia_Ads (Advertiser)**: Advertiser account with $148.50 advertising balance and live active campaigns.
- **SuperAdmin (Admin)**: Full administrative access to user directory, withdrawal queue, ad moderation, and global settings.

---

## 🌟 Implemented Features & Architecture

### 1. Public Homepage
- Hero section with live statistics ticker (Total Paid: \$1,482,910+, Active Members, Faucet Claims, Total Impressions).
- Supported Cryptocurrencies banner: Bitcoin (BTC), Ethereum (ETH), Tether (USDT TRC20), Litecoin (LTC), Dogecoin (DOGE), Tron (TRX), Solana (SOL).
- 3-step guide: Create Account, Complete Quick Tasks, Instant Withdrawal.
- Service cards for all earning streams and high-CTR advertiser features.

### 2. User Registration & Login
- Modal dialogs for instant sign-in and account registration.
- Account role selection (Earner or Advertiser).
- Welcome bonus credit (+150 Coins) upon registration.
- Password recovery request flow.

### 3. User Dashboard
- Real-time balances in internal Coins and USD equivalent.
- Level and EXP progress bar with automatic level-up logic.
- Loyalty streak multiplier status (+1% per consecutive day up to 100%).
- Available tasks counter (Faucet claims remaining, PTC ads available, Shortlinks available).
- Recent account activity table with live status badges.

### 4. Cryptocurrency Faucet
- 5-minute countdown timer with persistence across views.
- Interactive anti-bot math verification challenge.
- Dynamic loyalty streak calculation (Base 50 Coins + Loyalty streak bonus).
- Rewarding Web Audio chime and canvas confetti celebration on claim.
- Instant wallet balance update and transaction logging.

### 5. Paid-To-Click (PTC) Advertisements
- Filter tabs: All, Standard PTC, Window Ads, Iframe Ads, and YouTube Video ads.
- Live fullscreen Ad Viewer overlay modal:
  - Real-time countdown timer bar and visual progress indicator.
  - Active window focus detection for Window Ads (pauses automatically if user switches tabs).
  - Clean preview viewport for target URLs and embedded YouTube videos.
  - Anti-bot security code verification at completion.
  - Decrements advertiser impression budget and credits user balance in real-time.

### 6. Shortlinks Wall
- List of shortlink providers with rewards, EXP, and difficulty ratings.
- Safe, interactive 3-step transition simulation:
  - Step 1: 5-second preparation timer with progress bar.
  - Step 2: "I am not a robot" verification check.
  - Step 3: Unlocked reward claiming and instant balance update.

### 7. Offerwalls & Surveys
- Provider hub: CPX Research, BitLabs, Wannads, Monlix, Lootably, TimeWall.
- Sample offers for surveys, mobile games, and microtasks.
- Interactive 3-question survey taker simulator.
- Developer postback API simulator tool for testing server-to-server webhook deliveries.

### 8. Challenges & Achievements
- Daily and weekly challenge tracker with dynamic progress bars.
- Goals for Faucet claims, PTC views, shortlink completions, surveys, and weekly coin accumulation.
- One-click reward claim buttons.

### 9. 7-Day Daily Streak Bonus
- Visual 7-day calendar matrix with progressive rewards (25 to 500 Coins + Faucet Boost Ticket).
- Daily check-in claim button with next-claim debounce.

### 10. Referral System
- Unique referral link generator and referral code.
- 1-click clipboard copy and social share buttons (X/Twitter, Telegram, WhatsApp).
- Multi-tier commission structure (20% Faucet, 10% PTC, 10% Shortlinks, 5% Advertiser deposits).
- Ready-to-use HTML embed codes for Leaderboard (728x90) and Medium Rectangle (300x250) promotional banners.

### 11. Multi-Currency User Wallet
- Multi-currency live balances (Coins, USD, BTC, ETH, USDT TRC20, LTC, DOGE, TRX, SOL).
- Comprehensive Transaction History Ledger with filters (All, Faucet, PTC, Shortlinks, Withdrawals, Deposits).
- 1-click CSV transaction export.

### 12. Deposits & Payments
- Direct blockchain deposit generator (unique wallet addresses & vector QR code).
- FaucetPay Merchant instant deposit simulation.
- Deposit bonus incentive (+5% on deposits over \$20).
- "Simulate Successful Deposit" sandbox button for instant testing.

### 13. Withdrawals
- Supports BTC, ETH, USDT TRC20, LTC, DOGE, TRX, SOL.
- FaucetPay Micro-wallet: Minimum \$0.50 (500 Coins), 0% fee, instant API payout.
- Direct Blockchain: Minimum \$5.00 (5,000 Coins), standard network fee.
- Instant submission to the Admin Queue for approval or automated dispatch.

### 14 & 15. Advertiser Portal & Dashboard
- Dedicated advertising metrics: Ad Balance, Active Campaigns count, Delivered Impressions, Average CPC (\$0.0006).
- Campaign management table: pause, resume, delete, and view impression progress.

### 16 & 17. Create Advertisement & Live Platform Synchronization
- Campaign builder for PTC Standard, Window, Iframe, and YouTube formats.
- Duration options: 5s, 10s, 15s, 30s, 60s with dynamic pricing formula.
- Geo-targeting selection (Global, Tier 1, Tier 2).
- **Synchronous Integration**: Created campaigns appear immediately in the PTC Advertisements section for earners. When earners view them, remaining views decrement and advertiser balance updates in real-time.

### 18. Advertiser Payments & Funding
- Direct crypto deposit to ad balance.
- Internal transfer tool: convert earner coin balance into advertising balance with a **+5% bonus incentive**!

### 19. Campaign Reports & Vouchers
- Community promo code engine (redeem codes like `WELCOME100`, `CRYPTO2026`).
- Voucher creation tool for advertisers and admins.

### 20 & 21. Verification, Anti-Fraud & Profile Settings
- Anti-adblock detection banner.
- Anti-bot human verification challenges.
- Preset withdrawal addresses for FaucetPay and 6 major cryptocurrencies.
- Two-Factor Authentication (2FA) toggle.
- Active login sessions monitor.

### 22. Support & Information Pages
- Comprehensive categorized FAQ accordion.
- Live Payment Proofs table with clickable blockchain explorer mock links.
- Interactive Support Ticket system: submit tickets and reply to customer service threads.

### 23. Google AdSense & Sponsor Banners
- Clearly labeled Leaderboard (728x90) and Responsive bottom banners strictly separated from reward PTC tasks.
- Admin dashboard toggle to enable/disable network advertising.

### 24. SuperAdmin Dashboard Interface
- Platform metrics: Total Users, Active Ads, Platform Hot Wallet Reserve.
- User management: balance adjustments (+/- Coins), verify status, ban/unban toggles.
- Ad Moderation: approve, pause, or remove advertiser campaigns.
- **Pending Withdrawals Queue**: 1-click "Approve & Pay" (dispatches FaucetPay API) or "Reject & Refund".
- Global Settings: Faucet cooldown minutes, base reward coins, AdSense toggle, anti-adblock toggle.
- Anti-fraud security audit trail.

### 25 & 26. Appearance, Responsive Design & Frontend Interaction
- Dark / Light theme toggle.
- Modern glassmorphism UI with neon indigo, cyan, and emerald accents.
- Responsive for Desktop, Tablet, and Mobile devices (including mobile bottom navigation bar).
- Pure HTML5, CSS3, and JavaScript with Web Audio API sound effects and Canvas confetti.
