# Phase 1 Test Templates (v1)

Public raw URLs for the friend test of EA + Follow-up Desk + Research Assistant.

## Layout

```
templates/v1/
  pack-manifest.yaml          # EA reads this to know the pack and resume if interrupted
  ea-right-hand/
    template.yaml
    skills/ea-setup.md
  followup-desk/
    template.yaml
    skills/chase-nudge.md
  research-assistant/
    template.yaml
    skills/research-scan.md
  starters/
    phase1-test-starters.md   # short paste sentences for friends
```

## How friends use it

1. Create a fresh Grok Bot.
2. Paste only the short EA starter sentence (from starters/).
3. The EA fetches the manifest and templates, profiles once, creates Follow-up Desk then Research Assistant (staggered), and keeps checking completion if the user walks away.

## Research Assistant Firecrawl fallbacks

1. Use if already installed / MCP / plugin available.
2. Guide low-touch signup with referral + one-time API key paste (stored locally only).
3. Fall back to regular web search and note it.

The bot stays generic so the friend can keep and steer it.
