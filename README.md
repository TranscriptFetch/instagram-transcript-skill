# Instagram Transcript Skill

An agent skill that gives Claude Code, Codex, Cursor and other AI agents Instagram transcripts, through the [TranscriptFetch](https://transcriptfetch.com/?utm_source=github&utm_medium=skill&utm_campaign=instagram-transcript-skill) API.

- **Transcripts** of any public Instagram reel or video, by AI transcription of the audio, with timestamps
- **Find videos** by search or profile, with paging
- **Many at once**: up to 50 transcripts per request, or a whole profile
- **Ready for AI**: plain text (about two-thirds fewer tokens), Markdown with timestamp links, or chunks sized for embeddings

## Install

```bash
npx skills add TranscriptFetch/instagram-transcript-skill
```

Or copy the one file into Claude Code yourself:

```bash
mkdir -p ~/.claude/skills/instagram-transcript
curl -fsSL https://raw.githubusercontent.com/TranscriptFetch/instagram-transcript-skill/main/skills/instagram-transcript/SKILL.md -o ~/.claude/skills/instagram-transcript/SKILL.md
```

For other agents, put [`skills/instagram-transcript/SKILL.md`](skills/instagram-transcript/SKILL.md) in that agent's skills folder.

## First run

The first time you ask for a transcript, the agent opens a TranscriptFetch page in your browser. Sign in, check the code and click Approve. The agent gets its own API key, which never appears in the chat and which you can revoke on your API Keys page. No key to copy, no password shared with the agent.

## Try

- "Transcribe this reel: https://www.instagram.com/reel/..."
- "What are the steps in this Instagram recipe video? Give me a shopping list."
- "Get the last 20 reels from this profile with transcripts and find the ones about pricing."
- "Translate what this reel says into Spanish."

## Cost

50 free credits every month, no card. 1 credit per listing page; AI transcription is 1 credit per started 5 minutes of audio. Failed requests are free. Plans: [transcriptfetch.com/pricing](https://transcriptfetch.com/pricing?utm_source=github&utm_medium=skill&utm_campaign=instagram-transcript-skill).

## Other platforms

- [YouTube Transcript Skill](https://github.com/TranscriptFetch/youtube-transcript-skill)
- [TikTok Transcript Skill](https://github.com/TranscriptFetch/tiktok-transcript-skill)
- [MCP server](https://github.com/TranscriptFetch/youtube-tiktok-instagram-transcript-mcp) for YouTube, TikTok and Instagram transcripts in any MCP client
- [API docs](https://transcriptfetch.com/docs?utm_source=github&utm_medium=skill&utm_campaign=instagram-transcript-skill)

## License

MIT
