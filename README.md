# Prolific External Study Link – Getting Started

[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![Status: Beta](https://img.shields.io/badge/Status-Beta-orange.svg)]()
[![Purpose: Educational](https://img.shields.io/badge/Purpose-Educational-green.svg)]()

A minimal, end-to-end example showing how to programmatically create, publish, and analyze a survey on Prolific using the API.

This repository is designed as a getting-started demo for researchers, engineers, and AI/ML practitioners who want to quickly collect high-quality human responses using Prolific, often **within minutes of launching a study**.

## Files

- **[`config.yaml`](config.yaml)** - Survey configuration (questions, rewards, participant settings)
- **[`prolific_helpers.py`](prolific_helpers.py)** - Helper functions for Prolific API interactions
- **[`prolific-survey-getting-started.ipynb`](prolific-survey-getting-started.ipynb)** - Main notebook workflow
- **[`environment.yaml`](environment.yaml)** - Conda environment specification
- **[`.env.example`](.env.example)** - Template for environment variables

## Setup

1. Copy [`.env.example`](.env.example) to `.env` and add your Prolific API credentials:
   ```bash
   cp .env.example .env
   ```

   Required environment variables:
   - `PROLIFIC_API_TOKEN` - Your Prolific API authentication token
   - `PROLIFIC_WORKSPACE_ID` - Your workspace ID
   - `PROLIFIC_PROJECT_ID` - Your project ID

2. Install the required dependencies. For conda users, an [`environment.yaml`](environment.yaml) file is provided for convenience:
   ```bash
   conda env create -f environment.yaml
   conda activate rise_slides
   ```

## Usage

1. Edit [`config.yaml`](config.yaml) to customize your study
2. Run the [Jupyter notebook](prolific-survey-getting-started.ipynb) to create and publish your survey
3. View results with demographic breakdowns 

## Features

- Create surveys and studies via Prolific API
- Auto-publish and monitor submissions
- Visualize results by demographics
- Export data to CSV


## About Prolific

Prolific connects AI researchers and developers with high-quality human data. Source large samples of domain experts, experienced AI trainers, and diverse demographics in hours, not weeks.

- Documentation: https://docs.prolific.com/
- Get started today: https://app.prolific.com/

---

## Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

## Important Notice

> This project is provided **as-is** for **educational and research purposes only**.
> - 🔬 **Beta Status**: This is experimental code and may contain bugs or incomplete features
> - 📚 **Not Maintained**: No active development or support is provided
> - 🎓 **Educational Use**: Intended as a learning resource
> - ⚖️ **Use at Your Own Risk**: Test thoroughly before using in production environments
