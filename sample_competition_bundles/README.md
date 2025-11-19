## HOW TO EDIT THIS TEMPLATE BUNDLE FOR YOUR COMPETITION:

1. Replace scoring.py in sample_scoring_program with your own scoring program
2. Replace ingestion.py in sample_ingestion_program with your own ingestion program,
3. Replace files in sample_input_data and sample_reference_data with your files
4. Replace BDB_logo.png with your competition logo
5. Edit the competition.yaml to use your new image file instead of BDB_logo.png
6. Other edits like competition title, descriptions, and pages like participate and terms can be edited in the competition.yaml before upload, OR on the GUI following bundle upload.

Additional competition bundle examples are [here](https://github.com/codalab/competition-examples/tree/master/codabench) :

More specifically, if you want to building off of our provided example bundle, [this example bundle](https://github.com/codalab/competition-examples/tree/master/codabench/wheat_seeds/results_submission_bundle) has the same competition but with additional phases and solutions : 

## TO CREATE A COMPETITION

- From the front page [https://dev.bruindatabench.org/](https://dev.bruindatabench.org/) top menu, go to the Benchmark/Competitions
- Click the green “Upload” button at the top right.
- Upload the sample competition bundle => this will create your competition.

## TO MAKE A SUBMISSION

- In your competition page, go to the tab “My submissions”
- Submit the sample submission bundle.
- When your submission finishes, go to the Result tab to check it shows up on the leaderboard.

## TO MAKE CHANGES TO COMPETITION

- Click on the Edit gray button at the top the enter the editor
- Change the logo
- Save your changes

## Composition of the competition bundle

### metadata file

- competition.yaml: contains ALL the configurations of your benchmark/competition

### datasets

- sample_input_data: contains datasets for training models and datasets for testing models (i.e. X_train, y_train, X_test)
- sample_reference_data: answers to training Datasets (i.e. y_test)

### core logic

- sample_ingestion_program: defines the logic of how to read user submissions, read your data, train the model and inferences outputs
- sample_scoring_program: defines the logic of how to calculate user submissions score

### static files

- sample_participate_page.md: markdown file about how to participate in this benchmark/competition
- sample_terms_page.md: about the terms and conditions of the benchmark, this will show up when other participants join the benchmark/competition
- BDB_Logo.png: logo for this benchmark/competition

You are done with this simple tutorial.

Next, check the more [advanced tutorial](https://github.com/codalab/competitions-v2/tree/develop/docs/tutorial)
