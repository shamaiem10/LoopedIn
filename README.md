<div align="center">

# LoopedIn

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=26&pause=1200&color=0A66C2&center=true&vCenter=true&width=750&lines=%22Excited+to+announce...%22;an+automation+that+never+stops+hustling" alt="Typing SVG" />

![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![OpenRouter](https://img.shields.io/badge/OpenRouter-thought%20leadership-0A66C2?style=for-the-badge)
![Tavily](https://img.shields.io/badge/Tavily-fact--checked-00C2A8?style=for-the-badge)
![Discord](https://img.shields.io/badge/Discord-manager%20approval-5865F2?style=for-the-badge&logo=discord&logoColor=white)
![Buffer](https://img.shields.io/badge/Buffer-publish-1E88E5?style=for-the-badge)

### *"Humbled to introduce a project that changed how I think about content forever."*
*(it's a bot that writes LinkedIn posts about itself, if you must know)*

</div>

<br>

## What is this

**LoopedIn** is an n8n workflow that fully commits to the LinkedIn-thought-leader bit — on autopilot, every single day.

It studies your entire posting history so it never repeats a "here's what I learned from failure" post, drafts a brand new take, fact-checks itself so it doesn't get cooked in the comments, commissions an on-brand illustration, and sends it to you on Discord for final "approved by leadership" sign-off before it hits the feed.

No recycled hot takes. No stock handshake photos. Just a very committed autonomous intern who never runs out of things to say — and never posts without your yes.

<br>

## The daily grind

<div align="center">

| Step | What happens |
|:--|:--|
| **Clock-in** | Daily schedule trigger fires at 3PM |
| **Review history** | Reads every past post from Google Sheets |
| **Find the gap** | Buckets old posts by theme, picks the underused one |
| **Pitch an idea** | Scraps it and retries if it overlaps a past post |
| **Draft the post** | Full text, hook, and hashtags |
| **Fact-check** | Cross-references claims via live Tavily search |
| **Self-correct** | Quietly fixes anything that wouldn't survive the comments |
| **Commission art** | Generates a custom illustration for the topic |
| **File it away** | Uploads the art to Google Drive |
| **Request sign-off** | Sends draft + art to Discord |
| **Approved →** | Publishes live via Buffer |
| **Rejected →** | Logged and dropped, no one has to know |

</div>

<br>

## The cast of characters

<div align="center">

| Persona | Actually is |
|:--|:--|
| The Thought Leader | **n8n** — orchestrates the whole bit |
| The Ghostwriter | **OpenRouter** — writes the "vulnerable" posts |
| The Fact-Checker | **Tavily Search API** — keeps claims defensible |
| The Brand Designer | **Pollinations AI** — generates on-brand art |
| The Content Calendar | **Google Sheets + Drive** — tracks the persona |
| The Manager | **Discord** — final approval gate |
| The PR Team | **Buffer → LinkedIn** — pushes it live |
| The Asset Library | **Cloudinary** — hosts the graphics |

</div>

<br>

## The content calendar

Clone this Google Sheet structure:

<div align="center">

| Column | Meaning |
|:--|:--|
| `name` | Post title |
| `idea` | The "spicy take," short concept |
| `text` | Full ghostwritten post |
| `image` | Google Drive link to the art |
| `status` | `ready` → `posted` / `rejected` |

</div>

<br>

## Onboarding

1. Clone the Google Sheet with the columns above
2. Connect credentials:
   - Google Sheets OAuth2
   - Google Drive OAuth2
   - OpenRouter API
   - Tavily API
   - Discord Bot (guild + channel IDs)
   - Cloudinary (basic auth)
   - Buffer API
3. Set your Discord approval channel
4. Set your "peak engagement" posting hour
5. Activate the workflow — let it cook, you just supply the yes/no

<br>

## Why there's still a manager approval step

Every post is fact-checked and scored for originality before you ever see it — but nothing publishes without your explicit green light on Discord. Full autonomy on the tedious parts (research, drafting, art, damage control), full control on the one button that puts your name on it.

<br>

<div align="center">

### *"Grateful for this automation. It taught me that consistency beats perfection."*

<sub>built with an unreasonable number of `IF` nodes and zero shame</sub>

</div>
