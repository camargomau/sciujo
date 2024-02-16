---
date: 2023-01-08
type: 🧠
---

**Topics:** [[Notkesto]]

---

[obsidian-html](https://github.com/obsidian-html/obsidian-html) is the amazing tool that I use to convert my notes on Obsidian to an HTML-based website that's currently hosted on [notes.psycake.subspace.club](https://notes.psycake.subspace.club).

The `config.yml` that I use is:

```yaml
# Paths
obsidian_entrypoint_path_str: '<full local path to Index.md>'
html_output_folder_path_str: '<full local path>'
exclude_glob:
  - /output

# HTML output
site_name: Notkesto
html_custom_inclusions:
  - '<link rel="stylesheet" href="/obs.html/custom.css"/>'
  - '<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Inter"/>'
  - '<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=JetBrains+Mono"/>'
navbar_links:
  - name: '🏠️ Home'
    link: 'index.html'
  - name: '💻️ MAC'
    link: 'Mathematics/Matemáticas Aplicadas y Computación.html'
  - name: '👾 GitHub'
    link: 'https://github.com/camargomau/notkesto'
    type: external
file_exports:
  - encoding: binary
    src: '<full local path to favicon.ico>'
    dst: favicon.ico

# Features
toggles:
  process_all: true
  allow_duplicate_filenames_in_root: false
  no_clean: true
  features:
    styling:
      accent_color: '#337ba4'
	mermaid_diagrams:
	  enabled: false
    create_index_from_dir_structure:
      exclude_subfolders:
        - '.git'
        - '__src'
        - 'md'
        - 'obs.html'
        - 'Assets'
      exclude_files:
        - '.gitignore'
        - 'favicon.ico'
        - 'not_created.html'
        - 'CNAME'
        - 'README.md'
```

I additionally use a `custom.css` file to tweak the default look of the webpages. You can find this file in the [Notkesto's GitHub repo](https://github.com/camargomau/notkesto/blob/main/obs.html/custom.css) I wrote this file as of [version 3.4.0](https://github.com/obsidian-html/obsidian-html/releases/tag/v3.4.0) (it may break in the future).
