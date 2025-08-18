# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an educational repository containing an interactive Jupyter notebook series for learning t-distribution and t-tests in Korean. The project uses storytelling to teach statistical concepts, starting from the historical context of William Gosset's work at Guinness brewery in 1908.

## Development Commands

### Environment Setup
```bash
# Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Running the Notebooks
```bash
# Start Jupyter Lab
jupyter lab

# Alternative: Start Jupyter Notebook
jupyter notebook
```

### Development Workflow
```bash
# Install packages for development
pip install -r requirements.txt

# Verify installations
python -c "import numpy, pandas, scipy, matplotlib, seaborn, plotly, ipywidgets; print('All packages imported successfully')"
```

## Repository Structure

### Core Notebooks (Must be completed in order)
1. `01_normal_to_z_distribution.ipynb` - Introduction to normal distribution and Z-tests
2. `02_birth_of_t_distribution.ipynb` - Historical context and derivation of t-distribution
3. `03_types_of_t_tests.ipynb` - Three types of t-tests and their applications
4. `04_assumptions_and_violations.ipynb` - T-test assumptions and Welch's corrections
5. `05_real_world_applications.ipynb` - Practical applications and best practices

### Key Technologies
- **Data Processing**: numpy, pandas, scipy
- **Visualization**: matplotlib, seaborn, plotly (for interactive plots)
- **Interactive Elements**: ipywidgets for dynamic parameter adjustment
- **Statistical Computing**: scipy.stats for statistical distributions and tests
- **Progress Tracking**: tqdm for simulation progress bars

## Notebook Architecture

### Content Structure
Each notebook follows a consistent educational pattern:
- **Historical storytelling** to provide context
- **Interactive simulations** using Monte Carlo methods
- **Theoretical explanations** with mathematical foundations
- **Practical exercises** with real-world scenarios
- **Visual demonstrations** using plotly for interactivity

### Code Patterns
- Uses `np.random.seed(42)` for reproducible results
- Interactive widgets with `@interact` decorators
- Plotly subplots for comprehensive visualizations
- Korean language comments and outputs for educational clarity
- Monte Carlo simulations for conceptual understanding

### Statistical Concepts Covered
- Normal distribution and Central Limit Theorem
- Z-tests vs t-tests comparison
- Degrees of freedom (df = n-1) and its implications
- Student's t-distribution derivation
- One-sample, independent, and paired t-tests
- Assumption testing and violations
- Welch's t-test for unequal variances
- Effect sizes and power analysis

## Educational Philosophy

The project emphasizes:
- **Practical problem-solving** over theoretical abstraction
- **Historical context** to understand why statistical methods were developed
- **Interactive learning** through hands-on simulations
- **Visual intuition** before mathematical formalization
- **Real-world applications** in business, medicine, and research

## Working with This Repository

### When Modifying Notebooks
- Maintain the storytelling narrative flow
- Ensure all interactive widgets function properly
- Test Monte Carlo simulations with different parameters
- Verify mathematical formulas render correctly in markdown
- Keep Korean language explanations clear and educational

### Adding New Content
- Follow the established pattern of story → theory → simulation → practice
- Use consistent color schemes in visualizations
- Include both theoretical and empirical validation
- Provide clear learning objectives for each section

### Dependencies Management
All required packages are specified in `requirements.txt` with minimum versions to ensure compatibility with interactive features and Korean font rendering.