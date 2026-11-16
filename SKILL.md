---
name: indonesian-tech-creator
description: Use when creating tech content for Indonesian audience — ideation, scripting, optimization, scheduling, and monetization. Full workflow from idea to publish for TikTok, YouTube, Instagram, and blog.
version: 1.0.0
author: Ezha
license: MIT
tags:
  - content-creation
  - indonesia
  - tech
  - developer
  - social-media
  - youtube
  - tiktok
  - instagram
compatibility:
  - claude-code
  - codex
  - opencode
  - cursor
  - gemini-cli
  - github-copilot
  - hermes-agent
---

# Indonesian Tech Content Creator

Agent skill untuk developer Indonesia yang mau jadi tech content creator. Full workflow: ideation → scripting → optimization → scheduling → monetization.

## When to Use

Use this skill when:
- Planning tech content for Indonesian audience
- Writing scripts for TikTok, YouTube, Instagram Reels, or blog
- Creating Instagram carousels, Stories, or feed posts
- Optimizing titles, descriptions, hashtags for Indonesian market
- Creating content calendars
- Planning monetization strategy
- Analyzing content performance

## Core Workflows

### 1. Content Ideation

Generate 10-20 content ideas based on:
- Trending tech topics in Indonesia
- Target audience (junior/senior dev, students, professionals)
- Content format (TikTok, YouTube, blog, thread)
- Unique angle for Indonesian context

**Process:**
1. Ask user for: niche, target audience, platforms, timeframe
2. Scan trending topics (local tech news, social media, community discussions)
3. Filter by relevance and uniqueness
4. Generate ideas with: title, format, hook, why it works, unique angle
5. Prioritize by potential engagement

**Output format:**
```
📌 IDE #[number]: [Title]
- Format: [TikTok/YouTube/Blog/Thread]
- Hook: [Opening line]
- Why trending: [Reason]
- Unique angle: [What makes it different]
- Estimated effort: [Low/Medium/High]
```

### 2. Script Generation

Create complete scripts for any format:
- **TikTok/Reels** (15-60 seconds): Hook → Content → CTA
- **YouTube** (5-15 minutes): Intro → Main sections → Outro
- **Blog post**: Title → Intro → Sections → Conclusion
- **Twitter thread**: Hook → Points → CTA

**Indonesian context:**
- Casual tone (seperti teman cerita, bukan formal)
- Mix Bahasa Indonesia + English tech terms (yang umum)
- Reference local examples (Gojek, Tokopedia, Traveloka, local startups)
- Analogies that relate to Indonesian audience
- Include visual cues and text overlays for video

**Process:**
1. Ask user for: topic, format, duration/length, style, target audience
2. Generate structure based on format
3. Write script with timing/duration markers
4. Add visual cues (screen recordings, overlays, B-roll suggestions)
5. Include CTA and engagement hooks
6. Add notes: background music, posting time, hashtags

**Output format:**
```
🎬 [FORMAT] SCRIPT: [Title]
Duration: [X seconds/minutes] | Style: [Casual/Professional/Educational]

[0-X detik] HOOK
Visual: [What to show]
Audio: "[What to say]"
Text overlay: "[On-screen text]"

[X-Y detik] MAIN CONTENT
Visual: [What to show]
Audio: "[What to say]"
Text overlay: "[On-screen text]"

...

[Final seconds] CTA
Visual: [What to show]
Audio: "[What to say]"
Text overlay: "[On-screen text]"

---
📝 NOTES:
- Background music: [Suggestion]
- Caption: "[Ready-to-use caption with hashtags]"
- Post time: [Best time to post in WIB]
- Engagement: [How to boost engagement]
```

### 3. Title & Description Optimization

Generate optimized titles and descriptions for:
- YouTube: SEO + clickbait balance
- TikTok: Hook-focused, curiosity-driven
- Blog: SEO-optimized with keywords
- Instagram: Engaging + hashtags

**Process:**
1. Ask user for: topic, platform, target metrics (views, engagement)
2. Generate 5-10 title variations
3. Score each by: CTR potential, SEO strength, curiosity factor
4. Recommend top choice with reasoning
5. Generate: thumbnail text, tags, description first line

**Output format:**
```
🎯 [PLATFORM] TITLE OPTIMIZATION

Topic: [Topic]

TOP 5 TITLES (ranked by CTR potential):

1. "[Title]"
   - Score: [X/10]
   - Why: [Reasoning]
   - Keywords: [List]

...

---
📝 RECOMMENDED:
Title: #[number]
Thumbnail text: "[Text]"
Tags: [Comma-separated]
Description first line: "[First 150 chars]"
```

### 4. Content Calendar Planning

Create 2-4 week content calendar:
- Balance content types (educational, entertaining, promotional)
- Schedule by best posting times (Indonesian timezone)
- Integrate with Indonesian holidays/events
- Cross-platform coordination

**Process:**
1. Ask user for: platforms, posting frequency, niche, duration
2. Generate calendar with: day, content idea, platform, format
3. Add notes: posting times, content mix, engagement tactics
4. Include special dates (Harbolnas, Lebaran, etc.)

**Output format:**
```
📅 CONTENT CALENDAR: [Duration]
Niche: [Niche]

WEEK [X]:
┌─────────┬──────────────────────────────────────┬──────────┐
│ Day     │ Content                              │ Platform │
├─────────┼──────────────────────────────────────┼──────────┤
│ Senin   │ [Content idea]                       │ [Plat]   │
│ Selasa  │ [Content idea]                       │ [Plat]   │
│ ...     │ ...                                  │ ...      │
└─────────┴──────────────────────────────────────┴──────────┘

---
📝 NOTES:
- Best posting times: [Platform-specific times in WIB]
- Content mix: [Percentages]
- Engagement tactics: [How to boost]
- Cross-promote: [How to cross-post]
```

### 5. Monetization Roadmap

Create monetization strategy based on:
- Current follower count per platform
- Niche and audience
- Available monetization options (Indonesian market)

**Process:**
1. Ask user for: current stats (followers, views), niche, goals
2. Identify available monetization paths:
   - Affiliate programs (Indonesian: Niagahoster, Domain ID, etc.)
   - Platform funds (TikTok Creator Fund, YouTube AdSense)
   - Sponsorships (Indonesian brands, tech companies)
   - Digital products (ebooks, courses, templates)
   - Community/membership
3. Create roadmap: now → 3 months → 6 months → 12 months
4. Estimate revenue per stage
5. List action items

**Output format:**
```
💰 MONETIZATION ROADMAP

Your Stats:
- [Platform]: [X] followers
- Niche: [Niche]

CURRENT STAGE: [Stage name]

---
✅ AVAILABLE NOW:
1. [Monetization path]
   - Details: [How it works]
   - Estimated: [Revenue range]
   - Action: [What to do]

...

---
🎯 NEXT [X] MONTHS:
[Stage-by-stage plan]

---
📊 PROJECTION:
[Revenue estimates over time]

---
📝 ACTION ITEMS:
1. [ ] [Task] ([deadline])
2. [ ] [Task] ([deadline])
...
```

## Indonesian Context

### Audience Behavior
- Indonesian audience loves interaction (tanya-tanya, diskusi)
- Prefer casual tone over formal
- Mix Bahasa Indonesia + English tech terms is normal
- Price-sensitive: love "murah", "gratis", "hemat" angles
- Community-driven: Telegram groups, Discord servers, local meetups

### Best Posting Times (WIB)
- **TikTok**: 19:00-21:00 (peak), 12:00-13:00 (lunch)
- **YouTube**: 15:00-17:00 (afternoon), 19:00-21:00 (evening)
- **Instagram**: 12:00-13:00, 19:00-21:00
- **Blog**: Tuesday-Thursday, 09:00-11:00

### Local Examples & References
- Startups: Gojek, Tokopedia, Traveloka, Bukalapak, Akulaku
- Tech companies: Kata.ai, Nodeflux, Xendit, Ajaib
- Local cloud: Biznet Gio, Cloud Indonesia, IDCloudHost
- Payment: DOKU, Xendit, Midtrans, QRIS
- E-commerce: Tokopedia, Shopee, Bukalapak, Lazada

### Hashtag Strategy
**Indonesian tech hashtags:**
- #DeveloperIndonesia #TechIndonesia #ProgrammingIndonesia
- #CodingIndonesia #BelajarCoding #TutorialIndonesia
- #WebDev #JavaScript #Python #React #NodeJS

**Mix strategy:**
- 3-5 Indonesian hashtags
- 3-5 English tech hashtags
- 2-3 niche-specific hashtags
- 1-2 trending hashtags

## Monetization Programs (Indonesia)

### Affiliate Programs
- **Niagahoster**: Hosting, domain — Rp 50-100K per sale
- **Domain ID**: .my.id, .co.id — Rp 20-50K per sale
- **Udemy/Coursera**: Courses — 15-25% commission
- **JetBrains**: IDE licenses — Affiliate program
- **Figma**: Design tools — Affiliate program

### Platform Funds
- **TikTok Creator Fund**: 10K+ followers, 100K views/30 days
- **YouTube AdSense**: 1K subs + 4K watch hours
- **Instagram Bonuses**: Invite-only, high engagement

### Sponsorship Rates (Indonesian Market)
- **10-50K followers**: Rp 500K-2K per post
- **50-100K followers**: Rp 2-5K per post
- **100-500K followers**: Rp 5-15K per post
- **500K+ followers**: Rp 15-50K+ per post

## Examples

See `templates/` folder for ready-to-use templates:
- `tiktok-script-template.md`
- `youtube-script-template.md`
- `instagram-template.md` (Reels, Carousels, Stories, Feed)
- `blog-post-template.md`
- `content-calendar-template.md`

See `workflows/` folder for detailed workflow guides:
- `content-ideation.md`
- `script-generation.md`
- `title-optimization.md`
- `calendar-planning.md`
- `monetization-roadmap.md`

## License

MIT — Free to use, modify, and distribute.
