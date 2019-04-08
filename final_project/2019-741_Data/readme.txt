See the Project Description Document for more details on these files. As usual, contact the TA for clarification.
This readme describe the testing data format that will be used in the demo.

example_testing_data.txt shows the format for the testing data. Basically, the Y values are replaced by zero. The two queries included are the first two queries of the training data.
During the demo, your team will apply your model on similar test data file then output one of the following: 
- Format 1: A .csv file where each row contains "<Score>,<qid>" where <score> is used for ranking (what your model returns when applied on the data).
Note that this form is ``score descending'' where the largest score is ranked first, the second largest score is ranked second, and so on.
For example, the .csv of: 
5,1
8,1
2,1
Means that the second item in the test file is ranked first in query 1 since it has the highest score (8), the first item is ranked second in query 2, and third item is ranked third.

- Format 2: You can also replace the Y values in the data file .data where the null value, 0, is replaced by the score as well if that is easier.
For example: 
5 qid:1 1:0.1904762 2:0.093344346 3:6.4657204E-4 4:9.596929E-4 5:9.519016E-4 6:0.08552632 ...
8 qid:1 1:0.52380955 2:0.036228463 3:8.07117E-4 4:9.596929E-4 5:0.0010688262 6:0.016447369 ...
Meaning that the second item is ranked in front of the first item.