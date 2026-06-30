# Welcome to the DIP_IT Docs

<p align="center">
  <img src="img/logo.png" alt="Logo" width="500px">
</p>

DIP_IT is a MATLAB-based platform for direct infusion mass spectrometry data processing, filtering, normalization, visualization, and export.

The app is designed to support sequental and continuously acquisitioned data, blank and QC filtering, detecting adduct possible adducts and isotopologues, and downstream statistical analysis.

## Where to start

- Read the [Intallation](./getting-started/installation.md) page for details on how to install the application.
- Check out the [Your First Experiment](./getting-started/firstexperiment.md) page to see how you can get started on interpreting experiments.
- If needed, take a look at the documentation of the different features and settings, such as how to set [General Parameters](./documentation-of-features-and-settings/generalparameters.md) for peak detection and additional settings for [Defining Sections](./documentation-of-features-and-settings/sectiondefinition.md).

## Main capabilities

- Load `.raw` and `.mzML` mass spectrometry data
- Use log files to define samples, blanks, QC files, and continuous sections
- Detect sections from injection time or base peak/TIC thresholds
- Filter features by occurrence, blank signal, QC CV, S/N, and exclusion lists
- Normalize using TIC, targeted TIC, or internal standards
- Export filtered CSV and MetaboAnalyst-compatible tables
- Run PCA, volcano plots, ANOVA, heatmaps, correlation heatmaps, and dendrograms
- Search for targeted adduct and isotopologue evidence from scan-level data