
# Shared Task on Fine-Grained Toxicity Detection in Online Gaming (GameTox) at EEUCA 2026

Competition Link:

[Codabench](https://www.codabench.org/competitions/12083/)

**Toxicity Detection in Online Gaming Communities**

The prevalence of toxic behavior in online gaming communities necessitates robust detection methods to ensure user safety. This shared task focuses on detecting toxicity in game chat logs, specifically using the GameTox dataset, which captures the complex relationship between user intent and specific linguistic features. The objective is to develop systems that can classify the intent of a player's utterance (e.g., Hate, Threats, Non-toxic). The task utilizes 53,000 game chat utterances from *World of Tanks*.

## Task

**Intent Classification:** The aim is to classify the intent of a given game chat utterance into one of six categories. The dataset for this task uses the following labels: *Non-toxic*, *Hate and Harassment*, *Threats*, *Extremism*, *Insults and Flaming*, and *Other Offensive Texts*.

**To learn more about the dataset**: please refer to the [GameTox paper](https://aclanthology.org/2025.naacl-short.37/).

## Participation

Join our Codabench competition: [Codabench link](https://www.codabench.org/competitions/12083/)

## Dataset

All the utterances have a unique identifier called "index". The labels for training data are organized in the folder provided. For evaluation and testing, the submission format is mentioned below.

**Data**

  * [Training Data](https://drive.google.com/drive/folders/1HkfwexOpX1S9gRrMeCFMfZJjsBs0hQRu?usp=sharing)
  * [Evaluation Data (Without Labels)](https://drive.google.com/file/d/1tAks2vHCJqBjgv7-YeS6WE6XOYhRL9OP/view?usp=sharing)

## Use of External Data

The use of external datasets is permitted. You should also mention your external data usage in your paper write-up. Participants may find datasets such as the DotAlicious dataset (DOTA) or toxic comment datasets from Reddit/Twitter useful for transfer learning experiments.

## Evaluation

All the images have a unique identifier called "index". The labels for training data are organized in the folder provided. For evaluation and testing, the script takes one prediction file as input. 

Your submission file must be a .csv file named ‘predictions.csv’ with columns 'index' and ‘label’. You must zip this file and submit the zipped archive file. Ensure that the zip does not have any sub-directories or any files besides the 'predictions.csv' file. The system only recognizes the first file in the zip folder. Ensure that the index order in the submission file is in ascending order. A sample submission file is available [here](https://github.com/therealthapa/eeuca-toxicity/blob/main/sample_submission.csv).

| index | label |
|----------|----------|
|12345|	0|
|15001|	1|
|20524|	1|
|35231|	0|
|65102|	1|

The labels should be mapped to the following integers:

  * 0: *Non-toxic*
  * 1: *Insults and Flaming*
  * 2: *Other Offensive Texts*
  * 3: *Hate and Harassment*
  * 4: *Threats* 
  * 5: *Extremism* 

The performance will be ranked by **F1-score** (Macro).

## Sample Code

Sample code and the baseline models (e.g., Joint BERT, ToXCL) used for this dataset are available at our [GitHub Repository](https://github.com/shucoll/GameTox).

## Publication

Participants in the Shared Task are expected to submit a paper to the CASE 2026 workshop. Submitting a paper is not mandatory to participate in the shared task. Papers must follow the workshop submission instructions and will undergo regular peer review. Their acceptance will not depend on the results obtained in the shared task but on the quality of the paper. All the accepted papers will be published in the ACL Anthology.

## Timeline of the Events

  * Start of the Competition: Dec 10, 2025
  * Eval Phase Start: Dec 10, 2025
  * Test Phase Start: Jan 15, 2026
  * Test Phase End: March 15, 2026
  * Paper Submission Deadline: March 28, 2026
  * Notification of acceptance: April 28, 2026
  * Camera-ready paper due: May 12, 2026

## Organizers

- Surendrabikram Thapa (Virginia Tech, USA)
- Shuvam Shiwakoti (Virginia Tech, USA)
- Siddhant Bikram Shah (Northeastern University, USA)
- Kritesh Rauniyar (Delhi Technological University, India)
- Surabhi Adhikari (Columbia University, USA)
- Kristina T. Johnson (Northeastern University, USA)
- Hristo Tanev (European Commission, Joint Research Centre (EU JRC)
- Ali Hürriyetoğlu (Wageningen Food Safety Research, Netherlands)
- Usman Naseem (Macquarie University, Australia)

## Contact

If there are any questions related to the competition, please contact the organizers at rauniyark11@gmail.com. Participants in this shared task are encouraged to reach out with any concerns or questions to any of the shared task organizers.

## References

Naseem, U., Shiwakoti, S., Shah, S. B., Thapa, S., & Zhang, Q. (2025, April). GameTox: A Comprehensive Dataset and Analysis for Enhanced Toxicity Detection in Online Gaming Communities. In Proceedings of the 2025 Conference of the Nations of the Americas Chapter of the Association for Computational Linguistics: Human Language Technologies (Volume 2: Short Papers) (pp. 440-447).
