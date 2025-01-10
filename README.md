# Container Scan Tool

## Overview
The Container Scan Tool is designed to identify and extract component details from container images using Syft. It generates a well-formatted XLSX file with a summary of findings and detailed component information.

## Features
- Automates scanning of container images with Syft.
- Outputs an XLSX file with formatted component details.
- Provides a summary of findings in a styled table.

## Prerequisites
Ensure the following dependencies are installed:
- Python 3.6 or higher
- `syft` (CLI tool)
- Python libraries:
  - `argparse`
  - `subprocess`
  - `openpyxl`
  - `colorama`
  - `itertools`
  - `threading`

You can install the Python dependencies using pip:
```bash
pip install openpyxl colorama
```

## Usage
1. Clone this repository to your local machine.
2. Ensure `syft` is installed and available in your PATH.
3. Run the tool with the following command:
   ```bash
   python3 func.py -id <image_id>
   ```
   Replace `<image_id>` with the container image identifier you want to scan.

## Output
The tool generates an XLSX file in the `Output` directory with:
- A styled table of scanned components.
- A summary of findings (displayed from cells E3 to H7).

## Notes
- Ensure proper permissions for the `Output` directory.
- Review the generated XLSX file for detailed insights into your container image.

