# n8n Discord Anime Image Generator

Sanitized public example of an n8n workflow that:

- listens for a Discord command starting with `!anime`
- appends a style prompt
- sends the prompt to Fal text-to-image
- posts the generated image URL back to Discord

## Files

- `workflow.sanitized.json`: public-safe workflow export with IDs, instance references, webhook ID, and credential references redacted

## Before Importing

Replace the placeholder values in the workflow with your own:

- `YOUR_GUILD_ID`
- `YOUR_CHANNEL_ID`
- Discord credential setup
- Fal API authorization credential

## Notes

This repo intentionally contains a sanitized export only. Do not commit raw workflow exports that include real credentials or internal identifiers.