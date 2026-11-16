# YouTube Script Template

## Quick Reference
- Duration: 5-15 minutes (sweet spot: 8-12 menit untuk tutorial)
- Structure: Intro (30-60 detik) → Main Content (70% duration) → Outro (30-60 detik)
- Aspect ratio: 16:9 horizontal
- Key: Hook di 30 detik pertama, retention throughout

---

## Template

```
🎬 YOUTUBE SCRIPT: [Judul]
Duration: [X] minutes | Style: [Tutorial/Review/Discussion]

[0:00-0:30] INTRO - HOOK
Visual: [Kamu ke kamera / B-roll relevan / problem demonstration]
Audio: "[Hook yang grab attention + problem statement]"
Text overlay: "[Judul video / key question]"

[0:30-1:00] INTRO - CREDIBILITY & PREVIEW
Visual: [Kamu ke kamera]
Audio: "[Kenapa kamu qualified + apa yang akan dipelajari]"
Text overlay: "[Agenda / what you'll learn]"

[1:00-X:XX] SECTION 1: [Topic]
Visual: [Screen recording / slides / demo]
Audio: "[Penjelasan concept + contoh]"
Key points:
- [Point 1]
- [Point 2]
- [Point 3]

[X:XX-Y:YY] SECTION 2: [Topic]
Visual: [Live demo / walkthrough]
Audio: "[Step-by-step explanation]"
Key points:
- [Point 1]
- [Point 2]
- [Point 3]

[Y:YY-Z:ZZ] SECTION 3: [Topic]
Visual: [Advanced demo / common mistakes / tips]
Audio: "[Deep dive / best practices]"
Key points:
- [Point 1]
- [Point 2]
- [Point 3]

[Z:ZZ-END] OUTRO - SUMMARY & CTA
Visual: [Kamu ke kamera]
Audio: "[Recap + CTA: subscribe, comment, next video tease]"
Text overlay: "[Subscribe button / next video]"

---
📝 PRODUCTION NOTES:
- Thumbnail: [Description of thumbnail design]
- Title: [Final title]
- Description: [First 3 lines + timestamps + links]
- Tags: [Comma-separated tags]
- End screen: [Subscribe + next video]
- Cards: [Timestamps for key sections]
- Post time: [Day] [Time] WIB
```

---

## Example: Deploy Node.js Tutorial

```
🎬 YOUTUBE SCRIPT: Deploy Node.js ke Server Indonesia
Duration: 10 minutes | Style: Tutorial

[0:00-0:15] HOOK
Visual: Screen showing expensive AWS bill vs cheap local server
Audio: "Kamu masih deploy ke AWS yang mahal? Hari ini gue bakal tunjukin cara deploy Node.js ke server Indonesia cuma 50 ribu per bulan."
Text overlay: "DEPLOY NODE.JS CUMA 50RB/BULAN!"

[0:15-0:45] PROBLEM & CREDIBILITY
Visual: Kamu ke kamera
Audio: "Banyak developer Indonesia yang struggle dengan deployment. Mau pakai AWS mahal, mau pakai VPS luar negeri latency tinggi. Solusinya? Pakai server Indonesia. Gue udah pakai ini 2 tahun untuk production, dan hari ini gue bakal tunjukin step-by-step."
Text overlay: "2+ years production experience"

[0:45-1:00] PREVIEW
Visual: Slides showing agenda
Audio: "Di video ini kita bakal bahas: pertama, kenapa server Indonesia, kedua, setup server dari nol, ketiga, deploy aplikasi Node.js, dan terakhir, monitoring dan maintenance. Let's go!"
Text overlay: "Agenda: 1. Why local server 2. Server setup 3. Deploy Node.js 4. Monitoring"

[1:00-3:00] SECTION 1: WHY SERVER INDONESIA
Visual: Comparison table (AWS vs local)
Audio: "Pertama, kenapa harus server Indonesia? Tiga alasan: pertama, latency. User kamu di Indonesia, server juga di Indonesia, response time bisa di bawah 50ms. Kedua, harga. Server lokal 60-80% lebih murah dari AWS untuk spek yang sama. Ketiga, support. Bahasa Indonesia, payment lokal, dan paham regulasi Indonesia."
Key points:
- Latency: <50ms vs 200ms+
- Price: 50K vs 500K+ per month
- Support: Bahasa Indonesia, local payment

[3:00-5:30] SECTION 2: SERVER SETUP
Visual: Screen recording, step-by-step server setup
Audio: "Oke sekarang kita setup server. Gue pakai Biznet Gio karena murah dan reliable. Pertama, beli VPS, pilih Ubuntu 22.04. Kedua, SSH ke server. Ketiga, update system dan install dependencies. Keempat, setup firewall dan security."
Key points:
- Choose provider (Biznet Gio example)
- SSH access setup
- System update & dependencies
- Security: UFW firewall, fail2ban

[5:30-8:00] SECTION 3: DEPLOY NODE.JS
Visual: Screen recording, deploy process
Audio: "Sekarang deploy aplikasi Node.js. Pertama, install Node.js dan PM2. Kedua, clone repository kamu. Ketiga, install dependencies dan setup environment variables. Keempat, start aplikasi dengan PM2. Kelima, setup Nginx sebagai reverse proxy."
Key points:
- Install Node.js + PM2
- Clone repo & install deps
- Environment variables
- PM2 process manager
- Nginx reverse proxy

[8:00-9:30] SECTION 4: MONITORING
Visual: Screen recording, monitoring setup
Audio: "Terakhir, monitoring. Jangan sampai aplikasi down tapi nggak tahu. Kita pakai PM2 logs untuk check errors, dan setup simple monitoring dengan uptime robot. Plus, backup database otomatis setiap hari."
Key points:
- PM2 logs for errors
- Uptime monitoring
- Automated backups
- Performance monitoring

[9:30-10:00] OUTRO
Visual: Kamu ke kamera
Audio: "Jadi itu dia cara deploy Node.js ke server Indonesia cuma 50 ribu per bulan. Kalau kamu punya pertanyaan, comment di bawah. Jangan lupa subscribe untuk tutorial tech lainnya. Dan check link di description untuk daftar server Indonesia yang gue recommend. See you next time!"
Text overlay: "Subscribe + Link di description"

---
📝 PRODUCTION NOTES:
- Thumbnail: You pointing at server with text "DEPLOY NODE.JS\nCUMA 50RB!" with Indonesian flag
- Title: "Deploy Node.js ke Server Indonesia Cuma 50rb/Bulan! (Tutorial Lengkap)"
- Description: 
  "Belajar deploy aplikasi Node.js ke server Indonesia cuma 50rb/bulan. Tutorial lengkap dari setup sampai production!
  
  🔗 Link server: [affiliate link]
  📚 Source code: [GitHub link]
  
  Timestamps:
  0:00 Intro
  1:00 Why server Indonesia
  3:00 Server setup
  5:30 Deploy Node.js
  8:00 Monitoring
  9:30 Outro"
- Tags: node.js, deploy, server indonesia, tutorial, biznet gio, murah, hosting indonesia, vps indonesia, deployment, web development
- End screen: Subscribe button + next video "Setup Domain .my.id"
- Cards: 1:00, 3:00, 5:30, 8:00
- Post time: Rabu 16:00 WIB
```

---

## Tips for Indonesian Audience

1. **Hook kuat di 15 detik pertama**: Langsung tunjukin value/problem
2. **Bahasa casual tapi jelas**: Seperti ngajarin teman
3. **Visual yang jelas**: Screen recording harus readable, zoom in kalau perlu
4. **Contoh lokal**: Pakai Rupiah, reference company Indonesia
5. **CTA yang specific**: "Comment di bawah kalau punya pertanyaan" lebih baik dari "Jangan lupa comment"
6. **Timestamps di description**: Indonesian audience suka skip ke bagian yang mereka butuh
7. **Link affiliate di description**: Monetize tanpa ganggu content
