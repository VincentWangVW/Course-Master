# Course Master

Course Master is a Python-based application that helps users explore and analyze university courses. It features a GUI for user interaction, graph-based course dependency visualization, and a Scrapy-based web scraper for data collection.

## Features

- Visualizes course prerequisites using graph theory
- Simple GUI built with Tkinter for interaction
- Scrapes and stores course data using Scrapy
- Outputs course data in JSON format
- Includes a detailed PDF project report

## Installation

1. Clone this repository or unzip the archive.
2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

3. (Optional) If using the scraper, install Scrapy:

```bash
pip install scrapy
```

## Usage

### Run the GUI:
```bash
python main.py
```

### Run the web scraper:
```bash
cd course
scrapy crawl courses -o courses.json
```

### Visualize data:
Use the `visualization.py` and `graph.py` modules to process and visualize course relationships.

## Folder Structure

```
Course-Master-main/
├── main.py                  # Launches the GUI
├── gui.py                   # GUI logic
├── graph.py                 # Graph generation
├── visualization.py         # Visualization tools
├── requirements.txt         # Python dependencies
├── README.md                # Project overview
├── CSC111_Project_2_Report.pdf # Detailed project report
└── course/
    ├── scrapy.cfg
    ├── courses.json         # Scraped course data
    └── course/
        ├── spiders/
        │   └── courses.py   # Scrapy spider for course data
        ├── items.py, pipelines.py, settings.py
        └── ...
```

## Requirements

- Python 3.10+
- Scrapy
- Tkinter (usually preinstalled with Python)
- matplotlib, networkx

## Credits

Developed as part of a CSC111 course project. See `CSC111_Project_2_Report.pdf` for details.

---

© 2025 Course Master Contributors. All rights reserved.
