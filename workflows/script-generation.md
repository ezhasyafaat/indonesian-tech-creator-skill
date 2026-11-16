# Script Generation Workflow

## Overview
Create complete scripts for TikTok, YouTube, Instagram Reels, blog posts, and Twitter threads with Indonesian context.

## Process

### Step 1: Gather Requirements
Ask user for:
- **Topic**: What to create content about
- **Format**: TikTok, YouTube, Instagram Reel, Blog, Twitter thread
- **Duration/Length**: 
  - TikTok/Reels: 15-60 seconds
  - YouTube: 5-15 minutes
  - Blog: 1000-2500 words
  - Twitter: 5-15 tweets
- **Style**: Casual, professional, educational, entertaining
- **Target audience**: Junior dev, senior dev, students, etc.

### Step 2: Choose Template
Load appropriate template from `templates/` folder:
- TikTok: `templates/tiktok-script-template.md`
- YouTube: `templates/youtube-script-template.md`
- Instagram: `templates/instagram-template.md`
- Blog: `templates/blog-post-template.md`

### Step 3: Structure the Script

**For TikTok/Reels (15-60 seconds):**
```
[0-3 detik] HOOK
- Grab attention immediately
- State problem or make bold claim

[3-X detik] CONTENT (2-3 key points)
- Point 1 with visual/demo
- Point 2 with visual/demo
- Point 3 with visual/demo

[Final 5 detik] CTA
- Follow, save, comment
- Clear and specific
```

**For YouTube (5-15 minutes):**
```
[0:00-0:30] INTRO - HOOK
- Problem statement
- Why they should watch

[0:30-1:00] INTRO - CREDIBILITY
- Why you're qualified
- What they'll learn

[1:00-X:XX] SECTION 1
- Main concept
- Demo/example
- Key takeaways

[X:XX-Y:YY] SECTION 2
- Next concept
- Demo/example
- Key takeaways

[Y:YY-Z:ZZ] SECTION 3
- Advanced concept
- Demo/example
- Key takeaways

[Z:ZZ-END] OUTRO
- Summary
- CTA: subscribe, comment, next video
```

**For Blog (1000-2500 words):**
```
# Title (H1)
Intro (hook + what they'll learn)

## Section 1 (H2)
Content with code examples

## Section 2 (H2)
Content with screenshots

## Section 3 (H2)
Content with diagrams

## Conclusion (H2)
Summary + next steps + CTA
```

**For Twitter Thread (5-15 tweets):**
```
1/ Hook (make them click "Show this thread")
2/ Context/problem
3-10/ Main points (one per tweet)
11-14/ Additional tips/examples
15/ CTA (follow, retweet, comment)
```

### Step 4: Write the Script

**Key elements to include:**

**Visual cues:**
- What to show on screen
- Screen recordings
- Text overlays
- B-roll suggestions

**Audio:**
- What to say (word-for-word for TikTok/Reels)
- Tone and pacing
- Background music suggestions

**Text overlays:**
- Key points in large text
- Emojis for emphasis
- Consistent branding

**Indonesian context:**
- Casual tone (seperti teman cerita)
- Mix Bahasa Indonesia + English tech terms
- Local examples (Gojek, Tokopedia, etc.)
- Prices in Rupiah
- Reference Indonesian communities

### Step 5: Add Production Notes

Include:
- **Background music**: Genre, volume level
- **Caption**: Ready-to-use with hashtags
- **Post time**: Best time in WIB
- **Engagement tactics**: How to boost engagement
- **Thumbnail/cover**: Description for design

### Step 6: Review & Refine

Check:
- [ ] Hook is strong (first 3 seconds/first sentence)
- [ ] Content flows logically
- [ ] Visual cues are clear
- [ ] CTA is specific
- [ ] Indonesian context is natural
- [ ] Timing/duration is appropriate
- [ ] Hashtags are relevant (15-20 for Instagram)

## Example: TikTok Script

**Input:**
```
Topic: Git Tips
Format: TikTok
Duration: 45 seconds
Style: Casual
Target: Junior developer Indonesia
```

**Output:**
```
🎬 TIKTOK SCRIPT: Git Tips Senior Dev
Duration: 45 seconds | Style: Casual Indonesian

[0-3 detik] HOOK
Visual: Close-up ke kamera, ekspresi serius
Audio: "Kamu masih git add . setiap file? Senior dev nggak pernah gitu."
Text overlay: "STOP git add ."

[3-15 detik] TIP 1
Visual: Screen recording terminal
Audio: "Pakai git add -p. Ini interactive staging. Kamu bisa pilih hunk mana yang mau di-commit. Jadi commit kamu bersih."
Text overlay: "git add -p = selective staging ✅"

[15-27 detik] TIP 2
Visual: Screen recording
Audio: "Trus pakai git commit --amend. Lupa masukin file? Nggak perlu commit ulang. Amend aja."
Text overlay: "git commit --amend = fix last commit 🔧"

[27-40 detik] TIP 3
Visual: Screen recording
Audio: "Terakhir, git stash. Butuh switch branch tapi kerjaan belum selesai? Stash dulu, nanti di-apply lagi."
Text overlay: "git stash = save work in progress 💾"

[40-45 detik] CTA
Visual: Kembali ke kamera, senyum
Audio: "Follow untuk tips tech lainnya. Link di bio untuk tutorial lengkap."
Text overlay: "Follow @yourusername 🔥"

---
📝 PRODUCTION NOTES:
- Background music: Lo-fi coding beat, volume 20%
- Caption: "Git tips yang senior dev pakai 🔥 Save buat nanti! #DeveloperIndonesia #Git #Programming #CodingTips #TechIndonesia"
- Post time: Selasa 19:30 WIB
- Engagement: Pin comment "Mau tips apa lagi? Comment below!"
```

## Indonesian Tone Guide

**Do:**
- "Kamu" instead of "Anda" (more casual)
- "Nggak" instead of "tidak" (conversational)
- "Trus" instead of "terus" (natural speech)
- "Gue/lo" if targeting Jakarta audience
- Mix English tech terms naturally

**Don't:**
- Too formal (like reading news)
- Too slangy (hard to understand)
- Full English (lose local connection)
- Full Bahasa Indonesia (tech terms are usually English)

**Sweet spot:**
- 70% Bahasa Indonesia
- 30% English tech terms
- Casual but clear
- Like explaining to a friend

## Checklist

- [ ] Gathered all requirements (topic, format, duration, style, audience)
- [ ] Chose appropriate template
- [ ] Structured script with clear sections
- [ ] Wrote hook that grabs attention
- [ ] Added visual cues for each section
- [ ] Included audio/dialogue
- [ ] Added text overlays
- [ ] Included Indonesian context naturally
- [ ] Added production notes (music, caption, post time)
- [ ] Reviewed for flow and timing
- [ ] Checked hashtags (if applicable)
