# Install inctrl.ai on your iPhone

This guide walks you through installing **inctrl.ai** on an iPhone. The whole thing takes about 15 minutes the first time.

> **Before you start — two things to know:**
> - You need a **computer (Mac or Windows)** that you can keep turned on. It's required to install the app *and* to keep it working.
> - The app must be **refreshed every 7 days** (the computer does this automatically while it's on and near your phone). This is an Apple rule for apps installed outside the App Store — there's no way around it.

---

## What you need

- An iPhone
- A Mac or Windows computer
- An **Apple ID** — your existing one is fine. (If you'd rather not use your main account you can use a spare, but for installing a single app it makes no real difference. If you do make a new Apple ID, sign into iCloud with it once first, or AltStore may reject it.)
- A USB cable
- Both the iPhone and computer on the **same Wi-Fi network**

---

## Step 1 — Install AltServer on your computer

AltServer is the helper that installs apps onto your iPhone.

1. Go to [altstore.io](https://altstore.io) and download **AltServer** (for **AltStore Classic** — the free version). Do **not** get *AltStore PAL*; that's a separate paid EU marketplace app and won't work with this guide.
2. **Windows only:** also install **iTunes** and **iCloud** from Apple's website directly — *not* from the Microsoft Store (the Store versions don't work).
3. Open AltServer. It runs quietly in the **system tray** (Windows) or **menu bar** (Mac).

## Step 2 — Install the AltStore app on your iPhone

1. Plug your iPhone into the computer with the USB cable.
2. Unlock the iPhone and tap **Trust This Computer** (enter your passcode).
3. In **Finder** (Mac) or **iTunes** (Windows), turn on **"Sync this iPhone over Wi-Fi."**
4. Click the **AltServer icon** (tray/menu bar) → **Install AltStore** → choose your iPhone.
5. Enter your **Apple ID** and your **regular password** when asked.
   - If two-factor authentication is on, AltServer then asks for the **6-digit verification code** that pops up on your Apple devices — enter it. (Do **not** use an app-specific password; AltStore no longer accepts them.)
   - Tip: if this Apple ID is the same one signed into iCloud on this computer, you won't be asked for a code at all.
6. After ~30 seconds, **AltStore** appears on your home screen.

## Step 3 — Trust the app on your iPhone

1. Go to **Settings → General → VPN & Device Management**.
2. Under **DEVELOPER APP**, tap your **Apple ID email** → tap **Trust** → confirm.
   - Your iPhone must be connected to the internet for this to work.
3. **iPhone on iOS 16 or newer:** go to **Settings → Privacy & Security → Developer Mode**, turn it **On**, and restart when prompted.

## Step 4 — Add the inctrl.ai source and install

**Easiest (on the iPhone, after AltStore is installed):** tap this one-tap link — it opens AltStore and adds the source for you:

> **[Add inctrl.ai source to AltStore](altstore://source?url=https://raw.githubusercontent.com/Intelligence-Act/inctrl-ios-distribution/main/apps.json)**

Or scan this QR code **with the AltStore app already installed** (it deep-links into AltStore — it won't work as a plain camera scan before AltStore exists):

![Add source to AltStore QR code](https://api.qrserver.com/v1/create-qr-code/?size=220x220&data=altstore%3A%2F%2Fsource%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2FIntelligence-Act%2Finctrl-ios-distribution%2Fmain%2Fapps.json)

**Or add it manually:**

1. Open **AltStore** → **Browse** tab → tap **Sources** (top-right) → tap **+**.
2. Paste this source address and tap **Add Source**:

   ```
   https://raw.githubusercontent.com/Intelligence-Act/inctrl-ios-distribution/main/apps.json
   ```

3. **inctrl.ai** now appears in the Browse tab → tap **Install**.
4. Tap the **inctrl.ai** icon on your home screen to open it. 🎉

---

## Keeping the app working (the 7-day refresh)

The app stops opening after 7 days unless it's refreshed. To keep it working automatically:

- **Leave AltServer running** on your computer (set it to launch at startup).
- Keep your **iPhone on the same Wi-Fi** as the computer. AltStore refreshes the app in the background.

If the app ever won't open (you've been away from your computer for over a week):

1. Make sure AltServer is running and your iPhone is on the same Wi-Fi (or plug in via USB).
2. Open **AltStore → My Apps → Refresh All**.

---

## Good to know

- **3-app limit:** Apple allows only 3 apps installed this way per Apple ID (AltStore itself counts as one).
- **Your Apple ID is safe:** it's sent directly to Apple, not stored by AltStore. Using a spare Apple ID is still recommended.
- **Updates:** when a new version of inctrl.ai is released, AltStore shows an update badge — just tap to update.

---

## Trouble?

| Problem | Fix |
|---|---|
| "Unable to verify app" / "could not verify free of malware" | Connect the iPhone to Wi-Fi, then redo the **Trust** step (Step 3). |
| App won't open after a week | Refresh it (see *Keeping the app working* above). |
| Apple ID password rejected | Use an **app-specific password** (Step 2.5). |
| "Developer Mode" not visible | Only on iOS 16+. On older iOS it isn't needed — just do the Trust step. |
