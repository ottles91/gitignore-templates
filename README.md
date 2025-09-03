# Gitignore Templates

A collection of `.gitignore` templates for personal or team use. This repository provides both global ignores (OS/editor cruft) and project-specific templates to quickly get new projects set up.

## Structure

```text
gitignore-templates/
├── global/          # Global templates for OS and editors
│   ├── macos.gitignore
│   ├── windows.gitignore
│   └── editors.gitignore
├── projects/        # Language or framework-specific templates
│   ├── python.gitignore
│   ├── csharp.gitignore
│   ├── swift.gitignore
│   └── web.gitignore
├── default.gitignore
└── README.md
```

## Usage

Set a global ignore file so Git automatically ignores system and editor files across all your repos:

```bash
git config --global core.excludesfile ~/gitignore-templates/global/windows.gitignore
```

## Project-Specific Gitignore

Copy the relevant template into your project root:

```bash
cp ~/gitignore-templates/projects/python.gitignore .gitignore
```

You can also combine templates if needed:

```bash
cat ~/gitignore-templates/default.gitignore \
    ~/gitignore-templates/projects/python.gitignore > .gitignore
```

## Contributing

Feel free to submit PRs with additional templates, improvements, or updates. Keep templates clean and minimal—only include files that should truly be ignored.
