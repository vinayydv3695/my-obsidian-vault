# Blog Writing Guide

Complete guide to creating, formatting, and publishing blog posts with markdown, code snippets, and images.

---

## Quick Start

1. Create a new `.md` file in `/content/blog/`
2. Add frontmatter with metadata
3. Write your content in Markdown
4. Save and it appears automatically!

---

## Creating a Blog Post

### Step 1: Create the File

Files go in `/content/blog/`:

```
/content/blog/my-awesome-post.md
```

**File Naming Rules:**
- Use lowercase only
- Replace spaces with hyphens
- Keep it short and descriptive
- Use `.md` extension

**Examples:**
- ✅ `arch-linux-setup.md`
- ✅ `docker-tutorial.md`
- ❌ `My Awesome Post.md` (spaces, capitals)
- ❌ `post1.md` (not descriptive)

The filename becomes your URL:
- `docker-tutorial.md` → `/blog/docker-tutorial`

---

## Step 2: Add Frontmatter

Every post **must** start with frontmatter between `---` markers:

```yaml
---
title: "Your Post Title"
excerpt: "A compelling 1-2 sentence description"
date: "2026-01-18"
tags: ["Linux", "Tutorial", "DevOps"]
author: "Tanish Bhandari"
published: true
featured: false
coverImage: "/images/blog/cover.jpg"
videoUrl: "https://www.youtube.com/watch?v=VIDEO_ID"
---
```

### Frontmatter Fields Reference

| Field | Required | Type | Description |
|-------|----------|------|-------------|
| `title` | ✅ Yes | string | Post title (shows in listings and post header) |
| `excerpt` | ✅ Yes | string | Short description (150-200 chars, used in previews) |
| `date` | ✅ Yes | string | Publication date in `YYYY-MM-DD` format |
| `tags` | ✅ Yes | array | Categories for filtering (use existing tags when possible) |
| `author` | ❌ Optional | string | Author name (defaults to "Tanish Bhandari") |
| `published` | ❌ Optional | boolean | `true` to publish, `false` for drafts (default: true) |
| `featured` | ❌ Optional | boolean | Show in featured section (default: false) |
| `coverImage` | ❌ Optional | string | Path to cover image (shows in listing and top of post) |
| `videoUrl` | ❌ Optional | string | YouTube/video URL (adds "📺 Watch Video" link) |

### Common Tags

Use these for consistency:
- **Languages:** Python, JavaScript, TypeScript, Shell, Rust
- **DevOps:** Docker, Kubernetes, CI/CD, Ansible, Terraform
- **Linux:** Arch Linux, Customization, Tiling Managers, Desktop
- **Topics:** Tutorial, Advanced, Guide, Tips, Automation

---

## Step 3: Write Your Content

### Basic Markdown Syntax

#### Headings

```markdown
# Heading 1 (Main Title)
## Heading 2 (Sections)
### Heading 3 (Subsections)
```

**Note:** H2 and H3 headings automatically appear in the table of contents sidebar!

#### Text Formatting

```markdown
**Bold text**
*Italic text*
`inline code`
~~Strikethrough~~
```

#### Lists

```markdown
- Unordered list item
- Another item
  - Nested item

1. Ordered list
2. Second item
3. Third item
```

#### Links

```markdown
[Link text](https://example.com)
[Internal link](/about)
```

#### Blockquotes

```markdown
> This is a quote
> It can span multiple lines
```

---

## Adding Code Blocks

Code blocks support **syntax highlighting** for 50+ languages.

### Basic Code Block

````markdown
```bash
sudo pacman -S neovim
nvim ~/.config/nvim/init.lua
```
````

**Renders as:**
```bash
sudo pacman -S neovim
nvim ~/.config/nvim/init.lua
```

### Supported Languages

Common ones:
- `bash`, `shell`, `zsh`
- `python`, `javascript`, `typescript`
- `go`, `rust`, `java`
- `yaml`, `json`, `toml`
- `dockerfile`, `nginx`
- `sql`, `css`, `html`

### Code Examples

**Python:**
````markdown
```python
def greet(name: str) -> str:
    return f"Hello, {name}!"

print(greet("World"))
```
````

**Configuration Files:**
````markdown
```yaml
# docker-compose.yml
services:
  app:
    image: nginx:alpine
    ports:
      - "80:80"
```
````

**Inline Code:**
```markdown
Use the `docker ps` command to list containers.
```

---

## Adding Images

### Where to Store Images

Place images in `/public/images/blog/`:

```
/public/
  └── images/
      └── blog/
          ├── arch-setup-screenshot.png
          ├── terminal-preview.jpg
          └── architecture-diagram.png
```

### Cover Image (Thumbnail)

Shows in blog listing and at top of post:

```yaml
---
coverImage: "/images/blog/my-cover.jpg"
---
```

### Images Inside Blog Content

Use standard Markdown syntax:

```markdown
![Description of the image](/images/blog/screenshot.png)
```

**Example:**
```markdown
## Installation

First, download the ISO:

![Arch Linux download page](/images/blog/arch-download.png)

Then verify the signature...
```

### Image Best Practices

- **Use descriptive alt text** (helps accessibility and SEO)
- **Optimize file size** (keep under 500KB)
- **Use appropriate format:**
  - `.jpg` for photos
  - `.png` for screenshots with text
  - `.webp` for best compression
- **Descriptive filenames:** `hyprland-config-screenshot.png` not `img1.png`
- **Always start path with `/`:** `/images/blog/file.png`

### Image Examples

```markdown
![Terminal showing Neovim setup](/images/blog/nvim-terminal.png)

![System architecture diagram](/images/blog/architecture.png)

![Before and after comparison](/images/blog/before-after.jpg)
```

---

## Advanced Formatting

### Tables

```markdown
| Feature | Status | Notes |
|---------|--------|-------|
| Docker | ✅ Done | Working |
| K8s | 🚧 WIP | Testing |
| Ansible | ❌ Todo | Planned |
```

### Task Lists

```markdown
- [x] Install dependencies
- [x] Configure dotfiles
- [ ] Set up automation
- [ ] Write documentation
```

### Emojis

Use Unicode emojis directly:
```markdown
🚀 Deployment complete!
⚠️ Warning: Breaking changes
✅ All tests passed
```

---

## Complete Example Post

```markdown
---
title: "Setting Up Hyprland on Arch Linux"
excerpt: "Complete guide to installing and configuring Hyprland, the beautiful Wayland compositor with stunning animations and modern features."
date: "2026-01-18"
tags: ["Linux", "Arch Linux", "Hyprland", "Customization", "Tutorial"]
author: "Tanish Bhandari"
published: true
featured: true
coverImage: "/images/blog/hyprland-cover.png"
videoUrl: "https://www.youtube.com/watch?v=example"
---

# Setting Up Hyprland on Arch Linux

Hyprland is a modern, dynamic tiling Wayland compositor with stunning animations and excellent performance.

## Prerequisites

Before starting, ensure you have:
- Fresh Arch Linux installation
- Basic understanding of tiling window managers
- GPU with Wayland support

## Installation

Install Hyprland from the AUR:

```bash
yay -S hyprland-git
```

![Hyprland installation in terminal](/images/blog/hyprland-install.png)

## Configuration

Create the config file:

```bash
mkdir -p ~/.config/hypr
nvim ~/.config/hypr/hyprland.conf
```

Basic configuration:

```conf
# ~/.config/hypr/hyprland.conf
general {
    gaps_in = 5
    gaps_out = 10
    border_size = 2
    col.active_border = rgb(e91e63)
}

decoration {
    rounding = 10
    blur {
        enabled = true
        size = 3
        passes = 1
    }
}

animations {
    enabled = true
    bezier = myBezier, 0.05, 0.9, 0.1, 1.05
    animation = windows, 1, 7, myBezier
}
```

## Keybindings

Essential shortcuts:

| Key | Action |
|-----|--------|
| `SUPER + Return` | Launch terminal |
| `SUPER + D` | App launcher |
| `SUPER + Q` | Close window |

## Tips & Tricks

> **Pro Tip:** Use `hyprctl` to reload config without restarting

```bash
hyprctl reload
```

## Screenshots

Here's the final result:

![My Hyprland setup](/images/blog/hyprland-final.png)

## Conclusion

Hyprland offers the best of both worlds: beautiful animations and tiling efficiency. Enjoy your new setup! 🚀

**Resources:**
- [Hyprland Wiki](https://wiki.hyprland.org)
- [My Dotfiles](https://github.com/username/dotfiles)
```

---

## Publishing Workflow

### Drafts

Set `published: false` to work on drafts:

```yaml
published: false
```

Drafts are visible in development (`pnpm dev`) but hidden in production.

### Publishing

1. Write your post
2. Add images to `/public/images/blog/`
3. Test locally: `pnpm dev`
4. Set `published: true`
5. Commit and push to GitHub
6. Automatic deployment via Vercel/Netlify

---

## Troubleshooting

### Post doesn't appear

✅ Check `published: true`  
✅ Verify file is in `/content/blog/`  
✅ Ensure `.md` extension  
✅ Validate frontmatter syntax (proper YAML)

### Images not loading

✅ File exists in `/public/images/blog/`  
✅ Path starts with `/` (absolute path)  
✅ Filename matches exactly (case-sensitive)  
✅ File extension correct (`.png`, `.jpg`)

### Code not highlighting

✅ Language name is correct (lowercase)  
✅ Triple backticks properly closed  
✅ No extra spaces before backticks

### Frontmatter errors

✅ Three dashes `---` at start and end  
✅ Tags in array format: `["Tag1", "Tag2"]`  
✅ Date in quotes: `"2026-01-18"`  
✅ Booleans without quotes: `true` not `"true"`

---

## Tips for Great Blog Posts

1. **Start with a hook** - Grab attention in the first paragraph
2. **Use headings** - Break content into scannable sections
3. **Add visuals** - Screenshots, diagrams, code blocks
4. **Be practical** - Include working examples
5. **Test everything** - Verify code and commands work
6. **Proofread** - Check spelling and grammar
7. **SEO-friendly** - Use descriptive titles and excerpts

---

Happy blogging! ✍️
