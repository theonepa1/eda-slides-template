# EDA Slides Template

A template for creating data-driven presentations using Reveal.js and Chart.js.

## Project Structure

```
.
├── assets/                  # Shared assets for all 
│   ├── css/                 # CSS files
│   ├── js/                  # JavaScript files
│   │   ├── chart.min.js     # Chart.js library
│   │   └── reveal.js/       # Reveal.js library
│   └── fonts/               # Font files
├── projects/                # Individual presentation 
│   └── {project_name}/      # Project-specific directory
│       ├── data/            # Data files for the project
│       ├── agenda.md        # High-level presentation 
│       ├── detailed_plan.md # Detailed visualization plan
│       ├── instructions.md  # (Optional) Additional
│       └── index.html       # Generated presentation
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

1. **Create Agenda**: Run the command to create a high-level outline
   ```
   Create presentation for my_project
   ```
   This will generate `projects/my_project/agenda.md` with a structured outline.

2. **Create Detailed Plan**: Run the command to expand the agenda into a detailed plan
   ```
   Proceed to next step for my_project
   ```
   This will generate `projects/my_project/detailed_plan.md` with specific visualization details.

3. **Generate Slides**: Run the command again to create the final presentation
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

- Modern web browser (Chrome, Firefox, Safari, Edge)
- No server required - presentations work with local files

## License

This template is available under the MIT License.
