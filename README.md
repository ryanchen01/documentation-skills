# Agent Skills

A collection of practical agent skills for analysis and reporting tasks.

---

## Included Skills

### Analysis Report

**Location:** `skills/analysis-report/`

Generates comprehensive, structured research reports with a scientific approach. This skill enables agents to:

- **Explore & Map Projects** – Scan dependencies, identify physical models, and locate data files
- **Verify Data** – Execute analysis scripts and extract key metrics (performance, signal quality, statistics)
- **Generate Reports** – Produce structured Markdown reports with quantitative results, methodology documentation, and professional discussion sections

**Key Features:**
- Supports LaTeX-style formulas and isotopic notation
- Includes reference materials for domain-specific translations
- Outputs reports in Simplified Chinese by default
- Follows professional scientific writing standards

---

## Installation

### Install from GitHub

First, add this repository as a plugin marketplace in Claude Code:

```
/plugin marketplace add ryanchen01/skills
```

Then install the skills you need:

```
/plugin install analysis-report@agent-skills
```

### Local Development Installation

After cloning the repository, use the `--plugin-dir` parameter:

```bash
git clone https://github.com/ryanchen01/skills.git
claude --plugin-dir /path/to/skills
```

---

## Usage

After installation, simply describe your needs in Claude Code:

> "Analyze the stability of the sensor data in this repo."

> "Compare the simulation results between the 'Fast' and 'Accurate' algorithms."

> "Generate a comprehensive report comparing Method A vs Method B."

> "Extract key metrics from the experimental data and create an analysis report."

---

## Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository** and create your feature branch:

   ```bash
   git checkout -b feature/new-skill
   ```

2. **Add a new skill:**
   - Create a new folder under `skills/` (e.g., `skills/your-skill-name/`)
   - Include a `SKILL.md` file with instructions and examples
   - Add any necessary reference materials in a `references/` subdirectory

3. **Follow the skill structure:**

   ```
   skills/
   └── your-skill-name/
       ├── SKILL.md           # Skill definition and instructions
       └── references/        # Supporting materials (optional)
           └── ...
   ```

4. **Update the marketplace configuration:**
   - Add your skill to `.claude-plugin/marketplace.json`

5. **Submit a Pull Request** with a clear description of your changes.

### Guidelines

- Write clear, actionable instructions in your `SKILL.md`
- Include practical examples demonstrating skill usage
- Follow existing code style and documentation patterns
- Test your skill thoroughly before submitting

---

## License

This project is licensed under the **MIT License**.

Copyright (c) 2025 ryanchen01

See the [LICENSE](LICENSE) file for full details.
