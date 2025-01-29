# Theme Name: jungi

<img width="958" alt="image" src="https://github.com/user-attachments/assets/ef9b9841-6835-4eb8-987f-65090c8aa735" />

## Features

- Hierarchical navigation bar
- Single page applicagion

## Installation

```sh
git submodule add https://github.com/ijun17/hugo-theme-jungi.git themes/jungi
```

## Configuration

### directory.yaml

create `./data/directory.yaml`

```yaml
# example
- category: study
  sub:
    - category: programming \\ directory-example
```

In `directory.yaml`, only category and sub exist hierarchically. If the sub does not exist, post links will be created there. In the example above, links to posts are created under a folder named `directory-example`.

### hugo.toml

Add the settings below to `./hugo.toml`

```toml
theme = "jungi"

[params]
  author_name = "your name"
  author_bio = ["your bio 1", "...", "your bio n"]

[markup]
  [markup.highlight]
    noClasses = false

disableKinds = ["taxonomy", "taxonomyTerm"]
```
