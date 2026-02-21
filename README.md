# qpViz — qpAdm Admixture Visualizer

qpViz (repo: ad99/qpAdm-html-visualizer) is a lightweight, purely frontend web application designed to generate beautiful, publication-ready admixture charts from [qpAdm](https://github.com/DReichLab/AdmixTools) outputs.

With zero installation or backend dependencies required, you can simply open the HTML file in any modern browser, paste your `qpAdm` logs, and instantly export high-quality visualizations.

## ✨ Features

- **No Installation Required:** A 100% client-side, single-file HTML app. Runs entirely in your browser.
- **Flexible Input Parsing:** Easily paste raw `qpAdm` log text or a pre-formatted summary.
- **Beautiful Visualizations:** Generates clean, highly readable donut charts with data tables.
- **Customizable Aesthetics:**
  - **19 Color Palettes:** Includes standard research colors, ColorBrewer, colorblind-friendly options (Okabe-Ito, Paul Tol), and various aesthetic themes.
  - **Themes:** Toggle between Light and Dark mode cards depending on your publication or presentation background.
- **Multiple Layouts:** Choose from 5 different aspect ratios for various mediums (Default 16:10.5, Widescreen 16:9, Standard 4:3, Square, and Portrait).
- **Fine-Grained Controls:** Adjust donut hole size, toggle clockwise/counter-clockwise rendering, and enable/disable inline percentage labels.
- **One-Click Export:** Download the generated visual card directly as a PNG file.

## 🚀 How to Use

1. **Open the Tool:** Simply double-click on `qpAdm_html_visualizer.html` to open it in your preferred web browser.
2. **Input Data:**
   - **Paste** your raw `qpAdm` log or summary directly into the text area.
   - Alternatively, use the **Upload** button (`Ctrl+O`) to load your `.log` or `.txt` file.
3. **Generate Chart:** Click the **Generate** button or press `Ctrl+Enter`.
4. **Customize:** Use the toolbar settings to tweak the palette, aspect ratio, theme, and donut configuration until it fits your needs perfectly.
5. **Download:** Click the **↓ PNG** button to save the produced graphic.

## 📥 Supported Input Formats

### 1. Raw Log
You can paste the standard `.log` format output straight from `qpAdm`. The tool automatically identifies:
- Left populations / Target
- Best coefficients and standard errors
- Right populations (Outgroups)
- Statistics (p-value, chisq)

### 2. Compact Summary
If you prefer, you can use a condensed summary format, for example:
```text
Target: Population_Name
Weights:
PopA - 43.8% SE: 3.78% Z: 11.57
P value: 0.178 | chisq: 4.12 | Rights: Mbuti, Yoruba, ...
```

## 🛠 Built With

- **[Chart.js](https://www.chartjs.org/)** for the donut chart rendering.
- **[chartjs-plugin-datalabels](https://chartjs-plugin-datalabels.netlify.app/)** for inline chart data labels.
- **[html2canvas](https://html2canvas.hertzen.com/)** for rendering the DOM to a downloadable image.
- Pure HTML, CSS, and Vanilla JavaScript.

## 📄 License
This project is open-source. Feel free to modify the source code to fit your lab's specific formatting needs.
