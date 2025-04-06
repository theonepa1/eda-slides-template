# EDA Slides Template

A template for creating data-driven presentations using Reveal.js and Chart.js.

## Prerequisites

This template is designed to work with [Cursor IDE](https://cursor.sh/), a code editor with built-in AI capabilities. The presentation generation process relies on Cursor's AI agent to interpret your data and create the presentation.

## Project Structure

```
.
├── assets/                  # Shared assets for all presentations
│   ├── css/                 # CSS files
│   ├── js/                  # JavaScript files
│   │   ├── chart.min.js     # Chart.js library
│   │   └── reveal.js/       # Reveal.js library
│   └── fonts/               # Font files
├── projects/                # Individual presentation projects
│   └── {project_name}/      # Project-specific directory
│       ├── data/            # Data files for the project
│       ├── agenda.md        # (Generated) High-level presentation outline
│       ├── detailed_plan.md # (Generated) Detailed visualization plan
│       ├── instructions.md  # (Optional) Additional instructions
│       └── index.html       # (Generated) Final presentation
└── README.md                # This file
```

## How to Use

### 1. Create a New Project

Create a new directory under `projects/` with your project name:

```bash
mkdir -p projects/my_project/data
```

### 2. Add Your Data

Place your data files in the `projects/my_project/data/` directory. Supported formats:
- CSV files
- JSON files
- Other data formats (as needed)

### 3. (Optional) Add Instructions

If you want to provide additional guidance for the presentation generation, you can create an `instructions.md` file in your project directory:

```bash
touch projects/my_project/instructions.md
```

This file is completely optional and not required for the presentation generation process. You can use it to include:
- Specific visualization preferences
- Color schemes
- Additional context for the data
- Any other notes for the presentation generator

### 4. Generate the Presentation

The presentation generation process follows these steps:

1. **Create Agenda**: In the Cursor IDE chat, type the following prompt:
   ```
   Create presentation for my_project
   ```
   This will generate `projects/my_project/agenda.md` with a structured outline.
   
   **Review and Edit**: You can review and edit the agenda.md file before proceeding to the next step to customize the presentation structure.

2. **Create Detailed Plan**: In the Cursor IDE chat, type the following prompt:
   ```
   Proceed to next step for my_project
   ```
   This will generate `projects/my_project/detailed_plan.md` with specific visualization details.
   
   **Review and Edit**: You can review and edit the detailed_plan.md file before proceeding to the next step to customize the visualization details.

3. **Generate Slides**: In the Cursor IDE chat, type the following prompt again:
   ```
   Proceed to next step for my_project
   ```
   This will generate `projects/my_project/index.html` with the complete presentation.

### 5. View the Presentation

Open the generated `index.html` file in a web browser to view your presentation.

## Features

- **Data-Driven Visualizations**: Automatically generates charts and graphs from your data
- **Responsive Design**: Works on all screen sizes
- **Interactive Slides**: Built with Reveal.js for smooth transitions
- **Customizable**: Modify the HTML/CSS/JS to suit your needs
- **Self-Contained**: All assets are included locally

## Customization

### Themes

The presentation uses the white theme by default. To change the theme:

1. Modify the theme CSS link in `index.html`:
   ```html
   <link rel="stylesheet" href="../../assets/js/reveal.js/dist/theme/white.css">
   ```

2. Available themes include:
   - white.css
   - black.css
   - league.css
   - sky.css
   - beige.css
   - simple.css
   - serif.css
   - night.css
   - moon.css
   - solarized.css

### Chart Types

The template supports various chart types from Chart.js:
- Bar charts
- Line charts
- Pie charts
- Doughnut charts
- Radar charts
- Polar area charts

## Requirements

- [Cursor IDE](https://cursor.com/) with AI capabilities
- Modern web browser (Chrome, Firefox, Safari, Edge)
- No server required - presentations work with local files

## License

This template is available under the MIT License.
