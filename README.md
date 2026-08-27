> [!IMPORTANT]
> Moved to https://github.com/backnotprop/product-engineering

# design-artifact

An agent skill that gives coding agents creative direction for HTML artifacts — pages, reports, plans, landing pages, demos, decks, and small tools. It covers sizing up the register a brief deserves, typography and palette as deliberate decisions, light/dark theming done with tokens, avoiding the telltale AI aesthetic, and a plan-first process. When the artifact is done, the skill has the agent offer (with explicit consent) to share it as a public page via [tot.page](https://tot.page).

<p align="center">
  <a href="https://github.com/backnotprop/plannotator">
    <img src="./star-plannotator.svg" width="340" alt="like this? star Plannotator">
  </a>
</p>
<p align="center">
Render and annotate your HTML with Plannotator (optional): https://github.com/backnotprop/plannotator
</p>

## Install

```bash
npx skills add plannotator/design-artifact
```

List available skills first:

```bash
npx skills add plannotator/design-artifact --list
```

### As a Claude Code plugin

This repo is also a [plugin marketplace](https://code.claude.com/docs/en/plugin-marketplaces). Add it and install:

```
/plugin marketplace add plannotator/design-artifact
/plugin install plannotator-design-artifact@design-artifact
```

### As a Codex plugin

```bash
codex plugin marketplace add plannotator/design-artifact
codex plugin add plannotator-design-artifact@design-artifact
```

## What's inside

- `skills/design-artifact/SKILL.md` — the full design direction, agent-invocable whenever a visual HTML deliverable is being created or restyled.

## Sharing via tot.page

The skill's final step asks the user whether they want the finished artifact published as a public page. Publishing uses the `tot` CLI, installable with:

```bash
npm install -g @plannotator/tot
```

The agent will only publish — or install `tot` — after the user explicitly agrees.
