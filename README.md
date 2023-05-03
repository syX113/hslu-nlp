# HSLU: 
Contains the NLP project for the "Detecting greenwashing signals through a comparison of ESG reports and public media" challenge.
The analyzed datasets can be downloaded from the following Google drive:
https://drive.google.com/file/d/1D1qOuJvQx69afYyz4rwf2C-Nm0D4goKy/view?usp=sharing

Further information to the challenge/project can be found in the document in */docs* or the following links:
- https://www.swisstext.org/shared-task-1-detecting-greenwashing-signals-through-a-comparison-of-esg-reports-and-public-media/
- https://sites.google.com/view/greenwashingswisstext/home?authuser=0

### Run the analysis / EDA
- Clone the repository
- Download the data files to the */data* directory
- Install the requirements
- Run the preprocessing notebook (*stage1/00-data-preprocessing.ipynb*)
- Run the analysis notebook (*stage1/01-data-exploration-and-visualization.ipynb*)


### Repository structure

* [data/](./hslu-nlp/data) Data directory (download and store the datasets to this directory)
  * [checkpoints/](./hslu-nlp/data/checkpoints) Checkpoint directory to save intermediate processing steps.
  * [.gitkeep](./hslu-nlp/data/.gitkeep)
* [docs/](./hslu-nlp/docs) Contains the PDF with the project information
* [stage1/](./hslu-nlp/stage1) Contains the Juypter Notebooks for the data preprocessing/cleaning and the EDA
  * [00-data-preprocessing.ipynb](./hslu-nlp/stage1/00-data-preprocessing.ipynb)
  * [01-data-exploration-and-visualization.ipynb](./hslu-nlp/stage1/01-data-exploration-and-visualization.ipynb)
* [stage2/](./hslu-nlp/stage2)
  * [02-data-annotation.ipynb](./hslu-nlp/stage2/02-data-annotation.ipynb)
* [stage3/](./hslu-nlp/stage3) To-DO
* [stage4/](./hslu-nlp/stage4) To-DO
* [stage5/](./hslu-nlp/stage5) To-DO
* [.gitignore](./hslu-nlp/.gitignore)
* [README.md](./hslu-nlp/README.md)

Developed and authored by: Tim Giger