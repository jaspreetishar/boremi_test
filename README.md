# BoReMi
Bokeh-based jupyter-interface for Registering spatio-molecular data to related Microscopy images.

![BoReMi Logo](https://user-images.githubusercontent.com/103258471/197501791-dc7997a2-9e4e-44e9-ba6e-17af6dd57130.jpg)

## Play with the example data by clicking on the binder badge below! <br>No need for installation/ setup!

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jaspreetishar/boremi_test/main?urlpath=/lab/tree/Binder/GUI.ipynb)


## Example Data Sources -

- Sample HE images ([Repository Folder](https://github.com/jaspreetishar/boremi_test/tree/main/Binder/sample_images)):

  1. [Mouse brain H&E images](https://mouse.brain-map.org/experiment/siv?id=100142143&imageId=102162242&imageType=atlas&initImage=atlas&showSubImage=y&contrast=0.5,0.5,0,255,4)

- Sample DAPI image ([Repository Folder](https://github.com/jaspreetishar/boremi_test/tree/main/Binder/sample_images)):

  1. [Vizgen MERFISH mouse brain DAPI image](https://storage.cloud.google.com/public-datasets-vizgen-merfish/datasets/mouse_brain_map/BrainReceptorShowcase/Slice2/Replicate1/images/mosaic_DAPI_z2.tif)

- Sample Spatio-molecular data ([Repository Folder](https://github.com/jaspreetishar/boremi_test/tree/main/Binder/sample_spatial_data)):

  1. [Vizgen MERFISH mouse brain coordinates](https://storage.cloud.google.com/public-datasets-vizgen-merfish/datasets/mouse_brain_map/BrainReceptorShowcase/Slice2/Replicate1/cell_metadata_S2R1.csv)

  2. [Vizgen MERFISH mouse brain annotations](https://colab.research.google.com/drive/1OxJRO19cPsDW0JGAh4tLJjgOl7EMxQbP?usp=sharing&__hstc=30510752.4cb8d6b89fad2fa65d62bdaf607b6668.1649443550209.1649443550209.1649443550209.1&__hssc=30510752.10.1649443550210&__hsfp=2047326768&hsCtaTracking=070f4af1-2595-44c8-9779-4da89d538482%7Cf4313de5-25c4-4677-9fd6-82cf71d4fdc4#scrollTo=SDqqXPqBHpvx)


## Quick Start Guide: Setting up BoReMi on a Cluster or a Local Environment

1. Notebooks: To set up BoReMi, two notebooks are provided in the "BoReMi directory" on the repository's main page: GUI.ipynb and Functions.ipynb.
   - GUI.ipynb serves as a graphical user interface.
   - Functions.ipynb contains all the necessary functions.
  
2. Obtaining the notebooks: There are two methods to obtain the notebooks.
   - Direct Download: Click on "Code" at the upper right corner of this repository and select "Download ZIP". Move the downloaded .zip file to the desired directory on your local machine/cluster and unpack it.
   - Git Clone: Use the command "git clone https://github.com/jaspreetishar/BoReMi.git" to clone the repository and extract the notebooks onto your local machine/cluster.

3. Required Libraries/Packages/Extensions

   - Install Required Libraries/Packages/Extensions
     - Ensure you install the necessary libraries, packages, and extensions specified in the `requirements.txt` file located on the repository's main page using the following guidelines:
   
   - Create a New Virtual Environment
     - To avoid conflicts with existing versions of the required libraries/packages/extensions, it is recommended to create a new virtual environment. For instance, you can use Conda to create this environment:

     ```bash
     conda create --name boremi_env python=3.11.5
     conda activate boremi_env
     ```
     
   - Install Dependencies in the Virtual Environment
     - Once the virtual environment is activated, install the dependencies from the `requirements.txt` file:
     
     ```bash
     pip install -r requirements.txt
     ```
   - Update Regularly
     - Periodically check for updates to the `requirements.txt` file and update your virtual environment accordingly to stay compatible with the latest features and fixes.

   #### *By following these steps, you will ensure that BoReMi runs smoothly without any library conflicts, improving user experience.*
       
4. Accessing the GUI: To use BoReMi, open the notebook that contains the GUI. Type "jupyter-lab {absolute_address_of_the_GUI.ipynb}" in the terminal or an Anaconda command prompt.

5. BoReMi Usage: Follow the provided guidelines and instructions inside GUI.ipynb. Begin using the tool and explore its functionalities.

6. Exit: To exit the virtual environment, type "conda deactivate" in the terminal or an anaconda command prompt.
