# Data Viz & Dashboard — AI Prompt Generator

A free, standalone prompt-building tool for data visualization and dashboard design teams. No login required, no backend, works in any browser.

**Live tool:** [your-username.github.io/dataviz-prompt-generator](https://your-username.github.io/dataviz-prompt-generator)

---

## What it does

Guides you through 8 steps to build a complete, structured AI prompt for dashboards, reports, wireframes, and data visualizations. Copy the output and paste into Claude, ChatGPT, Gemini, or any AI tool.

### Steps
1. **Deliverable** — type, platform (Power BI, Tableau, Figma, etc.), canvas size
2. **Context** — industry, audience, problem statement, decision goals
3. **Features** — structural + interactive elements with "include now / maybe later" phasing
4. **Design direction** — visual style, theme, default layout, inspiration
5. **Pages** — up to 5 report pages, each with its own type, layout override, and metrics
6. **Audience & Accessibility** — WCAG compliance, colorblind-friendly, font size, etc.
7. **Brand** — hex codes, typography, brand guidelines
8. **Generate** — builds and copies the full prompt

---

## Setup — GitHub Pages (5 minutes)

1. Fork or clone this repo
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)` folder
4. Click Save — your tool will be live at `https://your-username.github.io/dataviz-prompt-generator`

That's it. No build step, no dependencies, no server.

---

## Setup — Local use

Just open `dataviz-prompt-generator.html` in any browser. Nothing to install.

---

## Using with Claude (Claude Project setup)

If your team has Claude Pro or Team accounts, you can add this as a Project artifact:

1. Create a new **Claude Project**
2. In the project, start a conversation and ask Claude to display the artifact
3. Pin the conversation for your team to reuse

Or paste the contents of `dataviz-prompt-generator.html` into a Claude conversation and ask:
> "Display this as an artifact I can use as a prompt builder tool"

---

## Customization

All options are in the single HTML file — no build process needed.

| What to change | Where in the file |
|---|---|
| Tool/platform options | `id="toolChips"` chip group |
| Page type options | `pageTypeOptions` array in the script |
| Visual style options | `id="visStyle"` select |
| Layout options | `layoutOptions` array + `id="layout"` select |
| Style reference links | Replace `[what's this?]` tooltip placeholder text |
| Team name / branding | `.app-header` in the HTML |

### Adding your style reference doc link

Find this section in the script and replace the placeholder text with your internal doc URL:

```html
<div class="tooltip-box">
  Placeholder — your team's style reference doc will be linked here.
  <!-- Replace with: <a href="YOUR_LINK">View style guide</a> -->
</div>
```

---

## Who this is for

- Data viz and BI teams prompting AI tools for dashboard design
- Designers using Power BI, Tableau, Looker, Figma, or coded dashboards
- Teams running an AI prompting challenge or skill-building program
- Anyone who wants better AI output without writing prompts from scratch

---

## Contributing

PRs welcome. If your team has additions — new page types, chart types, platform options, or style names — open an issue or submit a pull request.

---

## License

MIT — free to use, fork, and modify.
