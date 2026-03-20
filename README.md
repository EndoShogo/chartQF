# chartQF

An interactive web application for visualizing quadratic functions and equations as graphs. Users can input coefficients, manipulate curves through direct dragging, and overlay colored fill regions on the plot.

## Features

- Plot one or more quadratic curves simultaneously, each with an independent color
- Switch between quadratic function mode (y = ax^2 + bx + c) and quadratic equation mode (ax^2 + bx + c = 0)
- Enter coefficients in standard form (a, b, c) or vertex form (a, p, q)
- Drag the vertex marker to translate a parabola while preserving its shape
- Drag the scale handle to adjust the steepness of a curve while preserving its vertex
- Snap-to-zero: vertex coordinates snap precisely to the x-axis or y-axis when dragged within a defined pixel threshold
- Snap-to-grid: a lighter snap to the nearest tick mark on either axis, subordinate to snap-to-zero
- Add fill regions defined by x and y ranges, with selectable colors and configurable opacity
- Display discriminant, roots, vertex coordinates, and axis of symmetry in a result panel
- Scroll to zoom and drag to pan with a square grid maintained at all zoom levels

## Requirements

- Python 3.8 or later
- pip

## Installation

```bash
git clone https://github.com/EndoShogo/chartQF.git
cd chartQF
pip install -r requirements.txt
```

## Usage

```bash
python chartQF.py
```

Open a browser and navigate to `http://localhost:5000`.

## Project Structure

```
chartQF/
├── chartQF.py           # Flask application entry point
├── templates/
│   └── index.html       # Frontend: graph rendering, interaction logic
├── static/
│   └── style.css        # Stylesheet
└── requirements.txt     # Python dependencies
```

## Dependencies

| Package | Purpose |
|---|---|
| Flask | Web framework and routing |
| NumPy | Numerical computation |
| Matplotlib | Graph rendering (server-side, reserved for future use) |
| Plotly.js 2.27 | Interactive graph rendering in the browser (loaded via CDN) |

## License

This project does not currently specify a license. All rights reserved unless otherwise stated.
