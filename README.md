# Find-a-PhD

Structured collection of PhD (and postdoc) recruitment posts from professors on X/Twitter.

This repository is designed to power a daily-updated website that tracks faculty announcements about open PhD positions.

## Data Structure

### 1. PhD Recruitment Posts

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

### 2. 账号推荐 (Recommended Accounts)

Accounts that frequently post PhD recruitment information (personal professor accounts or aggregator accounts) are stored in `data/账号推荐.json`.

Structure:

| Field | Description |
|-------|-------------|
| `handle` | X/Twitter handle (e.g. @PhdScanner) |
| `type` | `aggregator` or `personal` |
| `name` | Display name |
| `description` | Short description of the account |
| `url` | Link to the profile |
| `notes` | Additional notes |
| `added_at` | When this account was added to the list |

Example entry already included: `@PhdScanner` (aggregator).

You can later continuously add more accounts to this file.

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

账号推荐数据:
```
https://raw.githubusercontent.com/jinzenshi/Find-a-PhD/main/data/%E8%B4%A6%E5%8F%B7%E6%8E%A8%E8%8D%90.json
```

## Future Automation

Planned: daily scrape of selected faculty accounts + automatic push of new/updated entries.

---

Maintained for personal PhD opportunity tracking + public website.
