# Identification Of Counterfeit Medicine Based On Appearance

This notebook presents a TensorFlow model that identifies counterfeit medicine based on appearance.  Specifically, the model receives image data as input and predicts the name (e.g., "Medithyl (10 mg)") and source (e.g., "Counterfeit D") of medicine in an image.  Organizations such as the [FDA](https://www.fda.gov/drugs/buying-using-medicine-safely/counterfeit-medicine) and [AAFP](https://www.aafp.org/fpm/2007/0300/p36.html) recommend such visual inspection as a simple method to identify counterfeits, which remain a persistent and deadly [global health risk](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4455087/).

<img src="https://www.pbs.org/wgbh/nova/media/images/lipitor-pills.width-1500.jpg" alt="Real Medicine Examples" width="400"/>

**Figure 1:** Counterfeit Lipitor pills (left) sit next to genuine examples (right).  This image and an associated article about counterfeit medicine are available on [PBS.org](https://www.pbs.org/wgbh/nova/article/uncovering-counterfeit-medicines/).

Due to limited availability of real-life counterfeit medicine images, our model is trained using approximately 5,100 near-photorealistic synthetic images.  These images were procedurally generated using Python, Blender, and GIMP. Ground truth labels were concurrently generated for each image and saved in a CSV file.

## Getting Started

### Prerequisites

This notebook requires a Python environment with the following modules and associated dependencies installed:

    jupyter
    matplotlib
    numpy
    pandas
    scikit-learn
    tensorflow

Interactive use of this notebook requires local notebook software such as [Jupyter](https://jupyter.org) or access to websites such as [Google Colab](https://colab.research.google.com).

## Usage

Run all cells in the notebook by selecting Cell > Run All (if using Jupyter locally) or Runtime > Run All (if using Colab).

The notebook will automatically download, explore, clean, and prepare the dataset before training and evaluating the TensorFlow model.  Numerous comments and cell outputs describe the steps being performed throughout the notebook.  The final output will include information and plots derived from the TensorFlow model's predictions on training, validation, and test datasets.  

## Credits

This notebook and all associated files were created by Davin C. (dc.ghub@gmail.com)

## License

This notebook and all associated files are Copyright (C) 2021 Davin C. (dc.ghub@gmail.com)