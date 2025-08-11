
## ✏️ Editing Content
Each section has a JSON file containing an array of objects.

Common fields:
- title (string, required)
- desc (string, optional)
- link (URL or relative path, optional)
- label (button text, optional; defaults to "Open" if link is present)

Example (songs.json):
```json
[
  { "title": "First Track", "desc": "Lo-fi groove", "link": "https://example.com/track1", "label": "Listen" },
  { "title": "Second Track", "desc": "Ambient pad" }
]
```

Workflow:
1. Open the repo → `content/` folder → pick e.g. `songs.json`.
2. Click the pencil (Edit) icon.
3. Add / edit objects (ensure valid JSON: commas only between items, none after the last item).
4. Commit changes ("Commit directly to main" is fine).
5. Refresh the live site and open that section. (Hard refresh with Cmd+Shift+R if old data shows.)

4. Save & commit. Visiting the new nav button loads JSON automatically.

## 🎵 Background Audio
- Place MP3 files in an `audio/` folder (create if not present).
- Add file paths to the `musicTracks` array in `index.html`.
- A random one plays (muted until first user interaction due to browser policy).

## ✅ Quick Edit Checklist
1. Open JSON file.
2. Add/remove an item object.
3. Validate brackets + commas.
4. Commit.
5. Refresh site & open section.

