# design-editor-skill

Agent skills for designing with [Design Editor](https://github.com/kemalcalak/design-editor): the `de` CLI, the batch design DSL, the MCP tools, the PenNode schema and UI design guidance, plus companion design and video skills.

## Install

With the editor's CLI installed:

```bash
de install            # detected agents
de install --target claude
```

Or add it to Claude Code as a plugin marketplace pointing at `kemalcalak/design-editor-skill`.

## Skills in this repo

**Design Editor**
- `design-editor`: how to build on the canvas over MCP or the `de` CLI. Start here.

**Design** (apply their principles on the canvas; ignore their HTML/React build steps)
- `design-dna`: extract a reference's tokens and style, then apply them.
- `frontend-design`, `design-taste-frontend`, `high-end-visual-design`, `minimalist-ui`, `industrial-brutalist-ui`: aesthetic direction and anti-template rules.
- `awesome-design-md`, `stitch-design-taste`: produce a `DESIGN.md`, which Design Editor imports directly (`set_design_md`).
- `impeccable`: critique and polish passes.

**Video** (turn designs into motion; export frames with `export_frames` and use them as assets)
- `hyperframes` (entry point), `hyperframes-core`, `hyperframes-animation`, `hyperframes-audio`, `hyperframes-cli`, `hyperframes-creative`, `hyperframes-keyframes`, `hyperframes-registry`, `hyperframes-studio`, `general-video`, `motion-graphics`, `product-launch-video`, `media-use`.
- `remotion-motion-graphics`: the same job with Remotion.

Sources and licenses: [THIRD_PARTY_NOTICES.md](./THIRD_PARTY_NOTICES.md).

## Also worth using (not bundled)

These are useful alongside Design Editor but are not included here, either because their license does not allow redistribution or because they target web code rather than the canvas. Install them from their own repositories:

| Skill | Use it for | Install |
|---|---|---|
| `web-design-guidelines` ([vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills)) | Auditing a built web UI against Vercel's interface guidelines | `npx skills add vercel-labs/agent-skills --skill web-design-guidelines` |
| `scroll-craft` ([nateherkai/scroll-craft](https://github.com/nateherkai/scroll-craft)) | Building the designed page as a scroll-driven website | `npx skills add nateherkai/scroll-craft` |
| `image-to-code`, `redesign-existing-projects`, `gpt-taste` ([Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill)) | Turning a design into code, or upgrading an existing site | `npx skills add Leonxlnx/taste-skill --skill <name>` |
| `imagegen-frontend-web`, `imagegen-frontend-mobile`, `brandkit` ([Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill)) | Generating design reference images or brand boards with an image model | `npx skills add Leonxlnx/taste-skill --skill <name>` |

## License

MIT for this repo's own content (see [LICENSE](./LICENSE)); bundled third-party skills keep their own licenses.
