# amlmarketplaces/vercel-ai

Claude Code marketplace federating all `@amlplugins/vercel-ai-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-vercel-ai": {
      "source": { "source": "github", "repo": "amlmarketplaces/vercel-ai" }
    }
  },
  "enabledPlugins": {
      "vercel-ai-amazon-bedrock@aml-vercel-ai": true,
      "vercel-ai-anthropic@aml-vercel-ai": true,
      "vercel-ai-azure@aml-vercel-ai": true,
      "vercel-ai-cerebras@aml-vercel-ai": true,
      "vercel-ai-cohere@aml-vercel-ai": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/vercel-ai`, cached under `~/.claude/plugins/cache/aml-vercel-ai/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (15 total)

- `vercel-ai-amazon-bedrock` — [@amlplugins/vercel-ai-amazon-bedrock](https://github.com/amlplugins/vercel-ai-amazon-bedrock)
- `vercel-ai-anthropic` — [@amlplugins/vercel-ai-anthropic](https://github.com/amlplugins/vercel-ai-anthropic)
- `vercel-ai-azure` — [@amlplugins/vercel-ai-azure](https://github.com/amlplugins/vercel-ai-azure)
- `vercel-ai-cerebras` — [@amlplugins/vercel-ai-cerebras](https://github.com/amlplugins/vercel-ai-cerebras)
- `vercel-ai-cohere` — [@amlplugins/vercel-ai-cohere](https://github.com/amlplugins/vercel-ai-cohere)
- `vercel-ai-deepinfra` — [@amlplugins/vercel-ai-deepinfra](https://github.com/amlplugins/vercel-ai-deepinfra)
- `vercel-ai-google` — [@amlplugins/vercel-ai-google](https://github.com/amlplugins/vercel-ai-google)
- `vercel-ai-google-vertex` — [@amlplugins/vercel-ai-google-vertex](https://github.com/amlplugins/vercel-ai-google-vertex)
- `vercel-ai-groq` — [@amlplugins/vercel-ai-groq](https://github.com/amlplugins/vercel-ai-groq)
- `vercel-ai-mistral` — [@amlplugins/vercel-ai-mistral](https://github.com/amlplugins/vercel-ai-mistral)
- `vercel-ai-openai` — [@amlplugins/vercel-ai-openai](https://github.com/amlplugins/vercel-ai-openai)
- `vercel-ai-openai-compatible` — [@amlplugins/vercel-ai-openai-compatible](https://github.com/amlplugins/vercel-ai-openai-compatible)
- `vercel-ai-replicate` — [@amlplugins/vercel-ai-replicate](https://github.com/amlplugins/vercel-ai-replicate)
- `vercel-ai-sdk` — [@amlplugins/vercel-ai-sdk](https://github.com/amlplugins/vercel-ai-sdk)
- `vercel-ai-togetherai` — [@amlplugins/vercel-ai-togetherai](https://github.com/amlplugins/vercel-ai-togetherai)

## Related

- npm packages: `@amlplugins/vercel-ai-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
