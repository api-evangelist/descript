# Descript (descript)

Descript is an AI-powered video and audio editing platform. Descript's API lets you programmatically create projects, import media, run AI ("Underlord") edits, publish compositions, and export transcripts — all without opening the desktop app. The API surfaces the same job model that backs the desktop editor and is currently in early access.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/descript/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - AI, Audio Editing, Captions, Media, Podcasting, Transcription, Video Editing

## Timestamps

- **Created:** 2026-05-06
- **Modified:** 2026-05-06

## APIs

### Descript Platform API

REST API for programmatically creating projects, importing media, running AI edits via the Underlord agent, publishing compositions, exporting transcripts, and managing asynchronous jobs in a Descript Drive. Authenticated with a personal Bearer API token scoped to a single Drive.

**Human URL:** [https://docs.descriptapi.com/](https://docs.descriptapi.com/)

**Base URL:** `https://descriptapi.com/v1`

#### Tags:

 - AI, Audio Editing, Jobs, Media, Projects, Publishing, Transcription, Video Editing

#### Properties

- [Documentation](https://docs.descriptapi.com/)
- [APIReference](https://docs.descriptapi.com/openapi-experimental.html)
- [OpenAPI](openapi/descript-openapi.yml)
- [Authentication](https://docs.descriptapi.com/#section/Authentication)
- [RateLimits](https://docs.descriptapi.com/#section/Rate-Limiting)
- [GettingStarted](https://docs.descriptapi.com/#tag/Getting-started)
- [CLI](https://www.npmjs.com/package/@descript/platform-cli)

## Common Properties

- [Portal](https://www.descript.com/api)
- [Documentation](https://docs.descriptapi.com/)
- [APIReference](https://docs.descriptapi.com/openapi-experimental.html)
- [SignUp](https://web.descript.com/signup)
- [Login](https://web.descript.com/login)
- [Pricing](https://www.descript.com/pricing)
- [Plans](plans/descript-plans-pricing.yml)
- [RateLimits](rate-limits/descript-rate-limits.yml)
- [FinOps Framework Profile](finops/descript-finops.yml)
- [CLI](https://www.npmjs.com/package/@descript/platform-cli)
- [Support](https://help.descript.com/)
- [Knowledge Center](https://help.descript.com/)
- [Blog](https://www.descript.com/blog)
- [YouTube](https://www.youtube.com/@descriptapp)
- [Terms of Service](https://www.descript.com/terms)
- [Privacy Policy](https://www.descript.com/privacy)
- [Security](https://www.descript.com/security)
- [GitHub Organization](https://github.com/descriptinc)

## Features

| Name | Description |
|------|-------------|
| Project Creation | Create new projects in a Drive and import media from public or pre-signed URLs in a single API request. |
| Direct File Upload | Receive 3-hour signed upload URLs from the import endpoint and PUT media bytes directly to storage. |
| AI Agent Editing | Send natural-language prompts to the Underlord agent to apply Studio Sound, captions, filler-word removal, translation, dubbing, and rough-cut building. |
| Asynchronous Jobs | All long-running operations return a job_id; clients poll GET /v1/jobs/{job_id} or supply a callback_url for webhook delivery. |
| Composition Publishing | Publish compositions to public, unlisted, drive, or private access levels with configurable resolution (480p–4K) for video. |
| Transcript Export | Export composition transcripts in txt, markdown, html, rtf, or docx with configurable speaker labels, markers, and timecodes. |
| Multi-Language Transcription | Automatically transcribe imported media in 25 languages with multi-speaker detection on paid plans. |
| Edit-in-Descript Partner Flow | Generate one-time import URLs for partner integrations so users can hand off media into Descript with a single click. |
| Published Project Metadata | Retrieve metadata (download URL, privacy, subtitles in WebVTT) for published projects via a public slug endpoint. |
| Rate-Limit Headers | 429 responses include Retry-After, X-RateLimit-Remaining, and X-RateLimit-Consumed for client-side budgeting. |

## Use Cases

| Name | Description |
|------|-------------|
| Podcast Production Automation | Import recordings, run Studio Sound and filler-word removal, and publish episodes without opening the desktop app. |
| Bulk Video Captioning | Programmatically caption a backlog of videos in 25 languages and export captions for downstream platforms. |
| AI-Driven Rough Cuts | Send raw multitrack recordings to the agent with a prompt like "build a rough cut" and retrieve a near-finished timeline. |
| Translation and Dubbing | Translate and dub video content into 30+ languages with proofread review using the Business plan's translation pipeline. |
| Content Repurposing | Generate clips, social cuts, and shorts from long-form recordings using Underlord prompts. |
| Embedded Video Workflows | Use the Edit-in-Descript partner endpoint to embed Descript editing into third-party recording tools (Ecamm, Restream, SquadCast, Zoom, Captivate). |

## Integrations

| Name | Description |
|------|-------------|
| Zoom | One-click import from Zoom recordings via Edit-in-Descript. |
| SquadCast | Multi-track remote recording handoff to Descript editing. |
| Restream | Live-stream recording capture with one-click import. |
| Ecamm | Mac live production handoff to Descript via Edit-in-Descript. |
| Captivate | Podcast recording and publishing integration. |
| YouTube | Direct publish target for finished compositions. |
| Slack | Embedded video playback and comment notifications via the Descript bot. |
| HubSpot | Publish destination for marketing video content. |
| Wistia | Publish destination for hosted business video. |
| Adobe Premiere / Audition | Timeline export targets for Adobe pro editors. |
| Final Cut Pro / DaVinci Resolve / Avid Pro Tools / Apple Logic / Reaper | Timeline export to professional NLEs and DAWs for finishing. |
| Buzzprout / Castos / Podbean / Podcast.co / Transistor / Captivate / Blubrry | Podcast hosting publish destinations. |
| Coursera | Educational publishing destination. |
| Google Drive | Cloud storage publish destination. |
| VideoAsk / Headliner / Hello Audio / eWebinar | Specialized publishing destinations for interactive video, audiograms, and webinars. |

## Compliance

| Name | Description |
|------|-------------|
| SOC 2 Type II | Audited SOC 2 Type II compliance. |
| GDPR | GDPR-compliant data handling with EU data subject rights honored. |
| CCPA | California Consumer Privacy Act-compliant. |
| Encryption | AES-256 at rest; TLS 1.2 in transit. |
| Data Deletion | Deleted projects are permanently removed within 30 days. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Descript Platform API](openapi/descript-openapi.yml) — OpenAPI 3.0.0, version 1.2 (early access)

### Plans

- [Descript Plans & Pricing](plans/descript-plans-pricing.yml) — API Commons Plans 0.1

### Rate Limits

- [Descript Rate Limits](rate-limits/descript-rate-limits.yml) — API Commons Rate Limits 0.1

### FinOps

- [Descript FinOps Profile](finops/descript-finops.yml) — FinOps Framework 1.0 (FOCUS-aligned)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
