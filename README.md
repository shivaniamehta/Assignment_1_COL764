# Assignment_1_COL764


1. Run invidx_cons.py to build Dictionary and Postings as

**python3 invidx_cons.py ./TaggedTrainingAP indexfile**

&nbsp;&nbsp; where, ./TaggedTrainingAP - denotes the folder that contains files of the collection

&nbsp;&nbsp; indexfile - name of the indexfiles

&nbsp;&nbsp; This will generate two files namely indexfile.dict (dictionary) and indexfile.idx ( Postings)

2. Run vecsearch.py to query and retrieve relevant documents

**python3 vecsearch.py topics.51-100 k resultfile indexfile.idx indexfile.dict**

&nbsp;&nbsp; where, topics.51-100 - name of the queryfile

&nbsp;&nbsp; resultfile - contains top k docids and their score in the treceval output format

&nbsp;&nbsp; k - top k number of relevant documents

&nbsp;&nbsp; indexfile.dict , indexfile.idx - as generated above

3. parseTags.py - used to identify the tagged terms in the document and merge the sequence of terms with same tags which belong to a single term
4. all.3class.distsim.crf.ser.gz and stanford-ner.jar - used to recognize named entities in the query
