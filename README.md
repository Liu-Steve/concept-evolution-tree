# Concept Evolution Tree (CET)

This repo is the official implementation of Concept Evolution Tree.

## Instruction

The dataset we are using is OpenAlex. To run this project, please refer to the [OpenAlex documentation](https://docs.openalex.org/download-all-data/openalex-snapshot) to download the dataset and use [this script](https://github.com/ourresearch/openalex-documentation-scripts/blob/main/flatten-openalex-jsonl.py) provided by OpenAlex to convert it to JSON Lines format. If downloading all of OpenAlex's data is too large for you, you can choose to use OpenAlex's API to download only the papers you need. Please ensure your final file is a text file where each line is a compact JSON string.

To run this code correctly, please follow these steps in sequence.

1. Follow the instructions in the file Topic_Modeling.ipynb to complete the Python environment configuration.
2. Run Paper_Screening.ipynb to select data into folder openalex_data. The folder should be created firstly.
3. Run Topic_Modeling.ipynb to perform topic clustering. You can modify the output_dir variable beforehand to distinguish different clustering result folders.
4. Run the EX1 file to build the concept evolution tree. The TOPIC_DIR variable can also be modified to determine which topic's data to use for plotting.

Files EX0 and EX2 are auxiliary experiments in the paper. EX0 can be run independently. For EX2, ensure that the file_path variable is modified after running Topic_Modeling.ipynb to find the corresponding data.
