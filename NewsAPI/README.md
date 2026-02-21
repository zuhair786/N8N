# Daily Football Video Generation — NewsAPI

Automated n8n workflow that generates a daily football highlights video using **NewsAPI** for news sourcing and **OpenAI GPT-4o** for content generation.

## How It Works

1. **Schedule Trigger** — Runs daily at 12:00 PM
2. **Fetch Football News** — NewsAPI pulls the latest football headlines
3. **Generate Video Prompt** — OpenAI GPT-4o creates a cinematic video prompt and image search queries
4. **Fetch Images** — Pexels API retrieves relevant football imagery
5. **Create Video** — Runway ML generates an image-to-video clip
6. **Poll for Completion** — Waits ~60s then checks Runway for the finished video

## APIs Used

| Service | Purpose |
|---------|---------|
| NewsAPI | Football news sourcing |
| OpenAI GPT-4o | Prompt generation |
| Pexels | Stock image retrieval |
| Runway ML | Video generation |

## Workflow Screenshot

![Workflow](daily_football_vedio_generation.png)
