# KoNA — project page

Project page for **Knowing What Not to Answer: Selective Non-Compliance in Vision-Language Models** (EMNLP 2026).

- Page: https://kona-emnlp2026.github.io/
- Paper: https://arxiv.org/abs/2609.04720
- Code: https://github.com/mz-kim/KoNA
- Dataset: https://huggingface.co/datasets/mz-kim/KoNA

## Structure

```text
index.html            page content
static/css/site.css   shared styles (same file in the RwR page repo)
static/css/page.css   page-specific components
static/js/site.js     shared behaviour: toggles, copy button, section highlighting
static/js/page.js     task examples, result data from the paper's tables, charts
static/img/           example images cropped from the paper's figures, social preview image, favicon
```

The page is plain HTML, CSS and JavaScript with no build step. Result numbers are copied from the camera-ready tables; `static/js/page.js` holds Table 2 and the ablation data. Example photos come from MS COCO and Open Images V7, as shown in the paper's figures.

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000/
```

GitHub Pages serves the `main` branch root.
