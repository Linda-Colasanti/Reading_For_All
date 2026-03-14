# Reading For All™ — Lesson System Guide
### How to publish a new lesson in 60 seconds

---

## Your Folder Structure

```
reading-for-all/
  lesson.html          ← NEVER touch this (the master template)
  lessons/
    1-1-short-a.json   ← one file per lesson
    1-2-short-e.json
    1-3-short-i.json
    ... and so on
  README.md            ← this file
```

---

## To Publish a New Lesson

1. Copy any existing `.json` file from the `lessons/` folder
2. Rename it to match the new lesson (e.g. `1-2-short-e.json`)
3. Open it and update these fields:

```json
{
  "lesson": "1.2",
  "title": "Short E",
  "subtitle": "with Abby & Otto",
  "pillar": 1,
  "level": 1,
  "character": "Otto",
  "brand": "Reading For All™",
  "youtube": "PASTE YOUTUBE EMBED LINK HERE",
  "fliphtml5": "PASTE FLIPHTML5 LINK HERE",
  "spotify": "PASTE SPOTIFY EMBED LINK HERE",
  "app": "PASTE GAME LINK HERE",
  "pdfs": [
    {
      "label": "📄 Download Worksheet",
      "description": "Practice Page",
      "url": "PASTE GOOGLE DRIVE OR PDF LINK HERE"
    }
  ],
  "description": "One sentence describing this lesson.",
  "whatYouWillLearn": [
    "Learning goal 1",
    "Learning goal 2",
    "Learning goal 3",
    "Learning goal 4"
  ]
}
```

4. Save the file to the `lessons/` folder in GitHub
5. Netlify auto-publishes within 60 seconds ✅

---

## How to Get Embed Links

| Content | Where to get the link |
|---|---|
| YouTube | Share → Embed → copy the `src="..."` URL only |
| Spotify | Share → Embed → copy the `src="..."` URL only |
| FlipHTML5 | Share → copy the page URL |
| Google Drive PDF | Share → Anyone with link → Copy link |
| Game/App | Just use the direct URL |

---

## Lesson Naming Convention

| Lesson | Filename |
|---|---|
| Pillar 1, Lesson 1 | `1-1-short-a.json` |
| Pillar 1, Lesson 2 | `1-2-short-e.json` |
| Pillar 2, Lesson 1 | `2-1-silent-e.json` |
| Pillar 3, Lesson 1 | `3-1-three-syllable-words.json` |

---

## Brand Colors (for reference)

- Navy: `#0d1b3e`
- Gold: `#f5c842`
- Rainbow: Red → Orange → Yellow → Green → Blue → Indigo → Violet

---

*Reading For All™ · LindaColasanti.com*
