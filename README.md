# Question_Classifier
-----------------------------------------------------------------

Decision Tree Classifier for classification of Questions in dataset

Features of Dataset:
-----------------------
 
(a) Length of the question

(b) Lexical Features: Word n-gram.

(c) Syntactic Features: Parts of speech tag unigrams.

- Model:
- 1,2,3 gram Language Models

Mapping for target class
{'ABBR': 0, 'DESC': 1, 'ENTY': 2, 'HUM': 3, 'LOC': 4, 'NUM': 5}
Datatset Attribute
------------------------------------------------------------------------------------------------------------------------
| Targte class | Raw Question | Question After preprocessing | length of question | Lexical | syntactical |
------------------------------------------------------------------------------------------------------------------------
--------------------------------------------------------------------------------------------------------------------------
first 5 rows from dataset after processing the question
Row 0
1
How did serfdom develop in and then leave Russia ?
['how', 'did', 'serfdom', 'develop', 'in', 'and', 'then', 'leave', 'russia']
9
None
None
Row 1
2
What films featured the character Popeye Doyle ?
['what', 'films', 'featured', 'the', 'character', 'popeye', 'doyle']
7
None
None
Row 2
1
How can I find a list of celebrities ' real names ?
['how', 'can', 'find', 'list', 'of', 'celebrities', 'real', 'names']
8
None
None
Row 3
2
What fowl grabs the spotlight after the Chinese Year of the Monkey ?
['what', 'fowl', 'grabs', 'the', 'spotlight', 'after', 'the', 'chinese', 'year', 'of', 'the', 'monkey']
12
None
None
Row 4
0
What is the full form of .com ?
['what', 'is', 'the', 'full', 'form', 'of', 'com']
7
None
None
first 5 rows from dataset after extracting lexical and syntactic data
Row 0
1
How did serfdom develop in and then leave Russia ?
['how', 'did', 'serfdom', 'develop', 'in', 'and', 'then', 'leave', 'russia']
9
['how', 'did', 'in', 'and', 'then']
['WRB', 'VBD', 'IN', 'CC', 'RB']
Row 1
2
What films featured the character Popeye Doyle ?
['what', 'films', 'featured', 'the', 'character', 'popeye', 'doyle']
7
['what', 'the', 'character']
['WP', 'DT', 'NN']
Row 2
1
How can I find a list of celebrities ' real names ?
['how', 'can', 'find', 'list', 'of', 'celebrities', 'real', 'names']
8
['how', 'can', 'find', 'list', 'of', 'real', 'names']
['WRB', 'MD', 'VB', 'NN', 'IN', 'JJ', 'NNS']
Row 3
2
What fowl grabs the spotlight after the Chinese Year of the Monkey ?
['what', 'fowl', 'grabs', 'the', 'spotlight', 'after', 'the', 'chinese', 'year', 'of', 'the', 'monkey']
12
['what', 'the', 'after', 'the', 'chinese', 'year', 'of', 'the']
['WP', 'DT', 'IN', 'DT', 'JJ', 'NN', 'IN', 'DT']
Row 4
0
What is the full form of .com ?
['what', 'is', 'the', 'full', 'form', 'of', 'com']
7
['what', 'is', 'the', 'full', 'form', 'of', 'com']
['WP', 'VBZ', 'DT', 'JJ', 'NN', 'IN', 'NN']
first 5 rows from training dataset after probability calculations
Row 0
1
How did serfdom develop in and then leave Russia ?
['how', 'did', 'serfdom', 'develop', 'in', 'and', 'then', 'leave', 'russia']
9
7.734196724847904e-08
0.00013266783798205007
Row 1
2
What films featured the character Popeye Doyle ?
['what', 'films', 'featured', 'the', 'character', 'popeye', 'doyle']
7
0.0013101844897959183
0.7824579360530675
Row 2
1
How can I find a list of celebrities ' real names ?
['how', 'can', 'find', 'list', 'of', 'celebrities', 'real', 'names']
8
2.7404778811929026e-13
2.4588954000112153e-05
Row 3
2
What fowl grabs the spotlight after the Chinese Year of the Monkey ?
['what', 'fowl', 'grabs', 'the', 'spotlight', 'after', 'the', 'chinese', 'year', 'of', 'the', 'monkey']
12
4.671329086249706e-10
0.08633452119520049
Row 4
0
What is the full form of .com ?
['what', 'is', 'the', 'full', 'form', 'of', 'com']
7
1.75915223862936e-12
0.02025786748867755
Mapping for target class
{'ABBR': 0, 'DESC': 1, 'ENTY': 2, 'HUM': 3, 'LOC': 4, 'NUM': 5}
Datatset Attribute
------------------------------------------------------------------------------------------------------------------------
| Targte class | Raw Question | Question After preprocessing | length of question | Lexical | syntactical |
------------------------------------------------------------------------------------------------------------------------
first 5 rows from dataset after processing the question
Row 0
5
How far is it from Denver to Aspen ?
['how', 'far', 'is', 'it', 'from', 'denver', 'to', 'aspen']
8
None
None
Row 1
4
What county is Modesto , California in ?
['what', 'county', 'is', 'modesto', 'california', 'in']
6
None
None
Row 2
3
Who was Galileo ?
['who', 'was', 'galileo']
3
None
None
Row 3
1
What is an atom ?
['what', 'is', 'an', 'atom']
4
None
None
Row 4
5
When did Hawaii become a state ?
['when', 'did', 'hawaii', 'become', 'state']
5
None
None
first 5 rows from dataset after extracting lexical and syntactic data
Row 0
5
How far is it from Denver to Aspen ?
['how', 'far', 'is', 'it', 'from', 'denver', 'to', 'aspen']
8
['how', 'far', 'is', 'it', 'from', 'denver', 'to', 'aspen']
['WRB', 'RB', 'VBZ', 'PRP', 'IN', 'NN', 'TO', 'VB']
Row 1
4
What county is Modesto , California in ?
['what', 'county', 'is', 'modesto', 'california', 'in']
6
['what', 'county', 'is', 'modesto', 'california', 'in']
['WP', 'NN', 'VBZ', 'NN', 'NN', 'IN']
Row 2
3
Who was Galileo ?
['who', 'was', 'galileo']
3
['who', 'was', 'galileo']
['WP', 'VBD', 'NN']
Row 3
1
What is an atom ?
['what', 'is', 'an', 'atom']
4
['what', 'is', 'an', 'atom']
['WP', 'VBZ', 'DT', 'NN']
Row 4
5
When did Hawaii become a state ?
['when', 'did', 'hawaii', 'become', 'state']
5
['when', 'did', 'hawaii', 'become', 'state']
['WRB', 'VBD', 'NN', 'NN', 'NN']
first 5 rows from testing dataset after probability calculations
Row 0
5
How far is it from Denver to Aspen ?
['how', 'far', 'is', 'it', 'from', 'denver', 'to', 'aspen']
8
5.4853999922335294e-08
0.0008350159563586373
Row 1
4
What county is Modesto , California in ?
['what', 'county', 'is', 'modesto', 'california', 'in']
6
1.1856409585819994e-06
1.5584426076095899
Row 2
3
Who was Galileo ?
['who', 'was', 'galileo']
3
0.058518982365854205
0.469523748848022
Row 3
1
What is an atom ?
['what', 'is', 'an', 'atom']
4
0.005470750385762961
0.7515745108399025
Row 4
5
When did Hawaii become a state ?
['when', 'did', 'hawaii', 'become', 'state']
5
2.907471246516451e-06
0.6002377132007415
/home/omkar/Dropbox/IITP/IITP_Assignment_Quiz/SEM1/AI/Assignment_4/dt.py:239:
VisibleDeprecationWarning: Creating an ndarray from ragged nested sequences (which is a list-or-tuple
of lists-or-tuples-or ndarrays with different lengths or shapes) is deprecated. If you meant to do this,
you must specify 'dtype=object' when creating the ndarray.
actual_target=np.array(test_data_after_prob_cal).T.tolist()[0]
gini
Building Tree ...
Predicting test data ...
Accuracy 41.2
ABBR 0| DESC 1| ENTY 2| HUM 3| LOC 4| NUM 5
precision [0.0, 0.18, 0.11920529801324503, 0.14213197969543148, 0.17142857142857143,
0.26666666666666666]
recall [0.0, 0.06521739130434782, 0.19148936170212766, 0.4307692307692308,
0.14814814814814814, 0.07079646017699115]
f-score [0.0, 0.09574468085106382, 0.1469387755102041, 0.2137404580152672,
0.15894039735099338, 0.11188811188811189]
support [9, 138, 94, 65, 81, 113]
entropy
Building Tree ...
Predicting test data ...
Accuracy 44.6
ABBR 0| DESC 1| ENTY 2| HUM 3| LOC 4| NUM 5
precision [0.0, 0.23255813953488372, 0.14507772020725387, 0.1568627450980392,
0.2033898305084746, 0.23076923076923078]
recall [0.0, 0.07246376811594203, 0.2978723404255319, 0.36923076923076925,
0.14814814814814814, 0.07964601769911504]
f-score [0.0, 0.11049723756906078, 0.19512195121951217, 0.22018348623853212,
0.17142857142857143, 0.11842105263157895]
support [9, 138, 94, 65, 81, 113]
ce
Building Tree ...
Predicting test data ...
Accuracy 50.1
ABBR 0| DESC 1| ENTY 2| HUM 3| LOC 4| NUM 5
precision [0.015625, 0.35135135135135137, 0.19402985074626866, 0.15, 0.2028985507246377,
0.20512820512820512]
recall [0.1111111111111111, 0.18840579710144928, 0.2765957446808511, 0.27692307692307694,
0.1728395061728395, 0.07079646017699115]
f-score [0.0273972602739726, 0.24528301886792453, 0.2280701754385965, 0.19459459459459458,
0.18666666666666665, 0.10526315789473684]
support [9, 138, 94, 65, 81, 113]
>>>
Q] Show whether errors propagated by one model are corrected by other
models or not. If yes, then report how many percent of samples are
corrected.
Ex. Observe how many samples are mis-classified using gini index based
model but correctly classified by mis-classification error and
cross-entropy based model.
samples misclassfied by gini but correctly classified by entropy 38
samples misclassfied by gini but correctly classified by ce 57
