# FlexMo

**FlexMo** contains the reproducible analysis notebooks associated with the manuscript:

*Cognitive Flexibility as a Potential Transdiagnostic Digital Biomarker Across Cognitive Aging Profiles: An Interpretable Multimodal Machine Learning Model That Integrates Features from Immersive Virtual Reality and Semantic Networks*

The manuscript is currently under submission.

## Overview

This repository provides the computational workflows used to derive, analyse, and interpret cognitive-flexibility markers from multimodal behavioural and language-based data. The analyses focus on Italian semantic-fluency responses, Picture Interpretation Test (PIT) narratives, and interpretable machine-learning models.

The repository contains the analysis files only. The datasets required to reproduce the analyses are archived separately on Zenodo.

## Repository contents

The repository includes three analysis notebooks:

1. **Semantic-fluency semantic-network workflow**  
   Preprocesses Italian verbal-fluency responses and derives semantic and lexical measures using SNAFU-based semantic-network procedures.

2. **Picture Interpretation Test NLP workflow**  
   Processes PIT narrative responses and extracts language-based variables for downstream analysis.

3. **Machine-learning and SHAP interpretation workflow**  
   Compares predictive models, identifies the selected best-performing models, and evaluates model interpretability using SHAP-based feature-attribution analyses.

## Data availability

The datasets used in these analyses are deposited on Zenodo.

Please download the required datasets from the corresponding Zenodo record and place them in the paths indicated at the beginning of each notebook before running the analyses.

Update this section with the final Zenodo DOI once the record is public or finalised.

## Reproducibility

Each notebook is intended to be run from top to bottom after the required input files have been downloaded from Zenodo. The notebooks define input paths, processing steps, intermediate outputs, and final analysis tables explicitly to support reuse and auditability.

For reproducibility, users should:

- use the same input files deposited on Zenodo;
- preserve the file names expected by the notebooks;
- run each notebook in order from the first cell to the last;
- record any changes to preprocessing, feature extraction, model selection, or interpretation steps.

## FAIR-oriented reuse

This repository follows FAIR-oriented documentation principles:

- **Findable:** the repository and Zenodo record provide persistent access points for the code and data.
- **Accessible:** analysis code is available through GitHub, while datasets are archived on Zenodo.
- **Interoperable:** workflows rely on standard Python notebooks and tabular data formats.
- **Reusable:** notebooks include explicit file names, documented processing steps, and analysis-ready outputs.

## Analysis workflows

### Semantic-fluency preprocessing and semantic-network measures

This notebook preprocesses Italian semantic-fluency responses and derives semantic and lexical measures. The workflow includes response cleaning, lexical harmonisation, preparation of analysis-ready tables, and computation of SNAFU-based semantic-network variables.

This workflow does not test associations with PIT outcomes. PIT responses are analysed separately in the NLP workflow.

### Picture Interpretation Test NLP analysis

This notebook processes free-text PIT responses and extracts linguistic variables from narrative descriptions. These variables are prepared for subsequent statistical or machine-learning analyses.

### Machine-learning model comparison and interpretation

This notebook compares multimodal predictive models against reference models. Models marked as selected correspond to the best-performing models retained for interpretation. SHAP analyses are used to examine feature contributions and support transparent model interpretation.

## Software requirements

The analyses are implemented in Python using Jupyter notebooks. Required packages are imported at the beginning of each notebook.

To run the notebooks, create a clean Python environment and install the required dependencies according to the imports listed in the notebooks.

Example:

```bash
python -m venv .venv
source .venv/bin/activate
pip install jupyterlab
jupyter lab
```

On Windows, activate the environment with:

```bash
.venv\Scripts\activate
```

Additional packages should be installed as required by the notebook import cells.

## Recommended use

1. Download the datasets from Zenodo.
2. Clone this repository.
3. Open the notebooks in JupyterLab or Jupyter Notebook.
4. Check and update the input paths at the beginning of each notebook.
5. Run each notebook from top to bottom.
6. Verify that generated outputs match the documented filenames and analysis steps.

## Citation

Please cite the associated manuscript once published.

> Pupillo, C. et al. *Cognitive Flexibility as a Potential Transdiagnostic Digital Biomarker Across Cognitive Aging Profiles: An Interpretable Multimodal Machine Learning Model That Integrates Features from Immersive Virtual Reality and Semantic Networks*. Manuscript under submission.

A full citation, DOI, and Zenodo record link should be added after publication or public release.

## License

Please add the appropriate software license before public reuse. If datasets are governed by separate access conditions, specify the data license or data-use restrictions in the Zenodo record.

## Contact

For questions about the analyses or repository, please contact the repository maintainer through GitHub.
