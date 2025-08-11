<style>
    body {
        background-color: #111;
        color: #eee;
        font-family: sans-serif;
        padding: 2rem;
        line-height: 1.6;
        text-align: center;
    }

    h1, h2, h3 {
        color: #66ccff;
        margin-top: 2rem;
        margin-bottom: 1rem;
    }

    p {
        max-width: 800px;
        margin: 0.5rem auto;
        text-align: left;
    }

    ul, ol {
        max-width: 9600px;
        margin: 1rem auto;
        text-align: left;
        display: table;
    }

    table {
        margin: 2rem auto;
        border-collapse: collapse;
        width: auto;
        max-width: 90%;
    }

    table th,
    table td {
        border: 1px solid #555;
        padding: 0.5rem 1rem;
        text-align: center;
    }

    video, 
    img {
        width: 90%;
        max-width: 960px;
        display: block;
        margin: 1rem auto;
        border-radius: 8px;
    }

    iframe {
        width: 90%;
        max-width: 960px;
        height: 500px;
        display: block;
        margin: 2rem auto;
        border: none;
        border-radius: 6px;
    }

    iframe.itch-widget {
        height: 167px !important;
        max-width: 960px;
        width: 90%;
        border-radius: 6px;
    }

    iframe.youtube-embed {
        width: 90%;
        max-width: 960px;
        height: 540px;
        display: block;
        margin: 2rem auto;
        border: none;
        border-radius: 6px;
        box-shadow: 0 0 12px rgba(0, 0, 0, 0.5);
    }

    a {
        color: #66ccff;
    }

    a:hover {
        text-decoration: underline;
    }

    pre {
        background-color: #1e1e1e;
        color: #f8f8f2;
        padding: 1rem;
        border-radius: 6px;
        text-align: left;
        max-width: 900px;
        overflow-x: auto;
        margin: 1rem auto;
        display: block;
        font-family: 'Courier New', Courier, monospace;
        font-size: 0.95rem;
        white-space: pre-wrap;
        box-shadow: 0 0 8px rgba(0, 0, 0, 0.4);
    }

    code {
        background-color: #2a2a2a;
        color: #ffecb3;
        padding: 0.2em 0.4em;
        border-radius: 4px;
        font-family: 'Courier New', Courier, monospace;
        font-size: 0.95em;
        white-space: pre-wrap;
    }

</style>

# GitHub Pages Template

This document presents a sample GitHub Pages layout that includes rich media such as:
- GIFs, Images & Videos
- `iframe` content from [YouTube](https://www.youtube.com/) , [itch.io](https://itch.io/) and [blueprintue](https://blueprintue.com/)

You can use this format to showcase games, prototypes, technical demos, or creative projects.

Please refer to the media and tables below as examples of how to present your work clearly and effectively.

---

## Markdown to HTML (`.md` → `.html`)

Once your [`index.md`](index.md) file is complete, you can convert it into a `.html` file using [VS Code](https://code.visualstudio.com/) and the [Markdown PDF](https://marketplace.visualstudio.com/items?itemName=yzane.markdown-pdf) extension:

1. Install **Markdown PDF** from the Extensions panel.
2. Open `index.md`.
3. Press `Ctrl + Shift + P` → Select **Markdown PDF: Export (html)**.
4. Commit the generated `index.html` file for use with GitHub Pages.

---

## Hosting via GitHub Pages

<iframe class="youtube-embed" src="https://www.youtube.com/embed/5XhxR9Vs6zc?si=ROTLf2RMwouvSjq2" allowfullscreen></iframe>

### Quick Hosting

1. Go to your repository on GitHub.
2. Click the **Settings** tab.
3. In the left menu, select **Pages** (under **Code and automation**).
4. Under **Build and deployment**:

   * Set **Source** to `Deploy from a branch`.
   * Set **Branch** to `main`.
   * Set **Folder** to `/ (root)` (or `/docs` if your content is in the `docs/` folder).
5. Click **Save**.
6. GitHub will generate a public URL (e.g.
   `https://your-username.github.io/your-repo-name/`) at the top of the page.

> Your site may take a minute or two to go live. Reload the link if you see a 404 error initially.

---

## Example GIF

![](assets/demo.gif)

*Figure 1. `demo.gif`, an example animated snippet showing system behaviour.*

GIFs are ideal for demonstrating short sequences, like UI transitions, animation loops, or gameplay snippets. Keep GIFs short and under 10MB where possible.

---

## Demo Video

<video controls>
  <source src="assets/demo.mp4" type="video/mp4">
</video>

*Figure 2. `demo.mp4`, a short embedded video demonstration.*

Videos are useful for showing interactions, effects, or walkthroughs. Use screen capture tools to create `.mp4` recordings of your project and embed them locally using the `<video>` tag.

---

## Blueprint Example

<iframe src="https://blueprintue.com/render/_wo11g40/" allowfullscreen></iframe>

*Figure 3. BlueprintUE embed — useful for sharing Unreal Engine logic visually.*

BlueprintUE is a powerful way to share and discuss Blueprint graphs in a readable format. Ideal for sharing logic behind player controls, mechanics, or UI interaction.

---

## Itch.io Widget

<iframe class="itch-widget" src="https://itch.io/embed/3456580" frameborder="0">
  <a href="https://simex.itch.io/hollowspire">Hollowspire by Simex, anstabo</a>
</iframe>

*Figure 4. Itch.io widget embed — link to downloadable or web-based projects.*

Use the Itch.io embed widget to allow others to play or download your game directly from your submission. This is useful for deployed games or interactive tools.

---

## YouTube Embed

<iframe class="youtube-embed" src="https://www.youtube.com/embed/XwYX2GLu6bU?si=AhM8-7fZvgBTXNOI" allowfullscreen></iframe>

*Figure 5. YouTube video — for trailers, walkthroughs, or demonstrations.*

If your video is hosted externally (e.g. YouTube), you can embed it directly using the iframe tag. This is especially useful for longer-form content or commentary.

---

## Code Snippet

```bash
# Example: clone and run
git clone https://github.com/yourusername/your-project-name
cd your-project-name
open index.html
```

*Figure 6. hello-world.cpp — for your... code...*

---

## Feature Summary

Use a table to summarise what your project contains:

| Feature              | Implemented | Notes                           |
| -------------------- | ----------- | ------------------------------- |
| Core Mechanic        | ✅ Yes      | Demonstrated via GIF/video      |
| UI/UX Functionality  | ✅ Yes      | Simple HUD layout shown         |
| Sound Implementation | 🔶 Partial  | Minimal SFX & Music, no settings|
| Save/Load System     | ❌ No       | Not required for this prototype |
| Gamepad Support      | ✅ Yes      | Tested with Xbox controller     |

*Figure 7. table example — use tables to show case data, features, etc*

