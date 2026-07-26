# Find-a-PhD

Structured collection of PhD (and postdoc) recruitment posts from professors on X/Twitter.

This repository is designed to power a daily-updated website that tracks faculty announcements about open PhD positions.

## Data Structure

All posts are stored in `data/phd_recruitment_posts.json` as an array of objects with the following fields:

| Field | Description |
|-------|-------------|
| `id` | X post ID |
| `post_time` | ISO 8601 timestamp of the original post |
| `author_name` | Full name of the professor |
| `author_handle` | X/Twitter handle |
| `institution` | University / Lab affiliation |
| `original_text` | Full original English (or original language) text |
| `chinese_translation` | Chinese translation of the post |
| `original_link` | Direct link to the X post |
| `research_focus` | Short summary of research area |
| `application_notes` | Key application info / deadlines |
| `scraped_at` | When this record was last updated |

## Recent Posts (as of 2026-07-25)

- **Yifat Prut** (Hebrew University) – ISF Breakthrough Grant, recruiting PhD + postdocs (Jul 23)
- **Andrea Ganna** (Human Technopole / PoliMi) – AI + foundation models + human genetics (Jul 22, apply by Sep 7)
- **Jason Chow** (Vanderbilt) – Fall 2027, education & equity / implementation science (Jul 19)
- Plus earlier posts from Sam Kumar (UCLA), Peter Henderson (Princeton), Yi Ma (HKU), Silja Häusermann (Zurich), Erik Sonnhammer (Stockholm)

## Usage for Website

You can fetch the latest JSON directly:

```
https://raw.githubusercontent.com/jinzenshi/Find-a-PhD/main/data/phd_recruitment_posts.json
```

## Future Automation

Planned: daily scrape of selected faculty accounts + automatic push of new/updated entries.

---

Maintained for personal PhD opportunity tracking + public website.
