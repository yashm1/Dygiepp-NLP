## T0 Download the dataset
1. Make a folder pretrained 
2. [Download the "coarse" model](https://ai2-s2-mechanic.s3-us-west-2.amazonaws.com/models/mechanic-coarse.tar.gz)
3. Paste the mechanic-coarse.tar.gz in the pretrained folder

## Setup 
1. conda create --name dygiepp python=3.7
2. conda activate dygiepp
3. pip install -r requirements.txt
4. conda develop .

This will add all the required packages to run the code

## To run the code
1.  cd Dygiepp-NLP in the repo
2.  RUN `allennlp predict ./pretrained/mechanic-coarse.tar.gz ./data/coarse/test.json --predictor dygie --include-package dygie --use-dataset-reader --output-file predictions/covid-coarse.jsonl --silent`
3.  The code will excute


## To Check the output
1. The output of the program will be in the `predictions/covid-coarse.jsonl`
