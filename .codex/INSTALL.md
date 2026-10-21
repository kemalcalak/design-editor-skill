# Installing Design Editor Skill for Codex

## Prerequisites

- Git

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/kemalcalak/design-editor-skill.git ~/.codex/design-editor-skill
   ```

2. **Create the skills symlink:**
   ```bash
   mkdir -p ~/.agents/skills
   ln -s ~/.codex/design-editor-skill/skills ~/.agents/skills/design-editor-skill
   ```

   **Windows (PowerShell):**
   ```powershell
   New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.agents\skills"
   cmd /c mklink /J "$env:USERPROFILE\.agents\skills\design-editor-skill" "$env:USERPROFILE\.codex\design-editor-skill\skills"
   ```

3. **Restart Codex** to discover the skills.

## Updating

```bash
cd ~/.codex/design-editor-skill && git pull
```

## Uninstalling

```bash
rm ~/.agents/skills/design-editor-skill
rm -rf ~/.codex/design-editor-skill
```
