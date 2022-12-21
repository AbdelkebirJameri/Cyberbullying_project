this project has a goal to detect offensive words in comments of social media , based on our labelization using doccano and implimenting Roberta model of Transformers ( huggingFace)

to use this :
- this folder contains out data ( already passed by Doccano for annotation ) format JsonL.
	dataproject.jsonl

- two jupyter notebook :
	-project_spliting daata.IPYNB : for processing of data  to transofrm the jsonL 	format to bert format ( contains tags and tokens ) 
	-Processing.IPYNB : this file contains all the process of tokenizationa ad 	traing our model based on Roberta of Transformers (huggingface)

- the feuture_class_labels.json : contails our labelization we extracted it in first jsonL to used it in the step of processing 

- file v1_annotated.json : this file contains extraxted after the step of spliting and processing the data , it's the good format  to use for Al bert model ( Roberta) and this is the file which we gonna use in the notebook of processing ( implimenting the model ). it contains tags and id and tokens of each word.

Please note : our model contains an error ( not an errors , just miss of training) while it shows 100% in the accuracy of the model :) :) , but we tried to host it using huggingface tokens classifiction API server , and it words it shows annotation of our words :) 
also we tried to impliment this project by passing in v1_annotated.json file which contains tags and tokens and we used the automatic tokens classification of hugging face ( also used Roberta) and actually work just fine with  top accuracy of traing of 83%. you can check this link : https://huggingface.co/abdelk/autotrain-tkc-2553578093?text=There+a+few+idiots+in+all+races.

I hope you understand the proccess.



Thank you so much for reading this note.

