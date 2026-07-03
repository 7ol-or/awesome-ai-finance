# Contribution Guidelines

Thank you for considering a contribution to **Awesome AI Finance**!

## Adding an Entry

Please ensure your suggested entry meets **all** of the following criteria before opening a pull request:

### ✅ Required

| Criterion | Detail |
|-----------|--------|
| **AI-first** | The tool uses LLMs, AI Agents, or advanced NLP as its core capability — not as a footnote or minor feature |
| **Finance scope** | Finance = trading / investing / portfolio management / market data / quant research. **Out of scope:** content monetization, social media automation, general "make money with AI" tools |
| **Active** | GitHub `pushed_at` within the past 12 months, or a widely recognized foundation project |
| **Not duplicated** | If a similar tool exists in the list, your entry must serve a meaningfully different purpose or have significantly more stars |
| **Open source** | Must have a public GitHub repository |

### License column

- Declared SPDX identifier (e.g. `MIT`, `Apache-2.0`) where available.
- `—` where GitHub reports no or unrecognized license. Use such repos at your own discretion.

### ❌ Not included

- Pure vector databases or embedding infrastructure
- RL/DL model training frameworks (e.g. FinRL)
- Traditional quant tools without AI at the core
- Plain stock/financial data APIs (no AI layer)
- Papers, courses, or educational resources
- Toy projects (very low stars, no meaningful user base)
- Archived or unmaintained repositories

## Format

One entry per row in the appropriate table section. Use this format:

```markdown
| [owner/repo](https://github.com/owner/repo) | One sentence describing the AI/LLM functionality, ending with a period. | ![Stars](https://img.shields.io/github/stars/owner/repo?style=flat-square) | YYYY-MM-DD | LICENSE |
```

- Description must end with a period.
- Description should focus on **what the AI does**, not just what the project is called.
- Place the entry in the most appropriate subcategory, sorted by stars descending.

## Updating an Entry

If a project has been updated significantly (new features, license change, star count has grown substantially), feel free to open a PR updating its description or position.

## Removing an Entry

If a project has been archived, abandoned (no commits in 12+ months), or deleted, please open a PR to remove it.

## Verification

All new entries are verified via the GitHub API for:
- `stargazers_count`
- `pushed_at` (recency)
- `license.spdx_id` (or `null` / `NOASSERTION`)
- `archived`

Please include the GitHub API output in your PR description to speed up review.
