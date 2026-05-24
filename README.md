# skills-repo

A curated, opinionated library of Claude skills for engineers, product managers,
and makers who ship things.

Each skill is a self-contained folder — drop it into your Claude setup and get
best-practice reasoning, structured outputs, and real-world templates for every
stage of the product lifecycle.

No fluff. Every skill ships with a quality bar baked in.

---

## Structure

```
skills-repo/
├── engineering/          # Code review, system design, API design …
├── software-engineering/ # ADRs, incident response, refactoring …
├── product-management/   # PRDs, roadmaps, user stories …
├── productivity/         # OKRs, decisions, async updates …
└── templates/            # Standalone reusable templates
```

## Using a skill

Copy the skill folder into the `skills/user/` directory of your Claude
installation, then reference it in your workflows.

## Adding a skill

1. Create a folder under the appropriate category
2. Add `SKILL.md` with YAML frontmatter (`name`, `description`)
3. Optionally add `references/`, `assets/`, `scripts/`
4. Open a PR with a sample output in `assets/example.md`

---

*Quality bar: every skill must include at least one real-world sample output.*
