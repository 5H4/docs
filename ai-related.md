## Ai Products recommendation.

### Segments

	- Related product:
		- required imports
			- collections
			- pandas
			- difflib
			- requests
			- dir src.app".py" -> recommend func.
				- from sklearn.feature_extraction.text import TfidfVectorizer [Alghoritm]
				- from sklearn.metrics.pairwise import linear_kernel [Alghoritm]
		- API request param: sku=$sku$ type= [json, ui]
			- get related product of target sku.
		- Minimum prod. quantity is 5
		- Minimum target prod. quantity is 5
		- [ZOHO != OMG] skip prod.

- Sklearn machine learning
	- [Sklearn Documentation](https://scikit-learn.org/)

- The TF*IDF algorithm is used to weigh a keyword in any document and
	assign the importance to that keyword based on the number of times it
	appears in the document. Put simply, the higher the TF*IDF score (weight),
	the rarer and more important the term, and vice versa.
	- [TF DF Documentation](https://en.wikipedia.org/wiki/Tf%E2%80%93idf)

#### Slovenian

- method 
	- [a][e][i][o][u] color, items [done] with difflib
	- [Samoglasnik](https://sl.wikipedia.org/wiki/Samoglasnik)

#### Translate natural language to English

- method
	- googletrans [API Doc](https://cloud.google.com/translate/docs/)
	- exmp: say denarnica - > wallet
	- for non english better is model method -> tested

#### Constructor

- Get from [speech, chat] keyword multiple keyword set + 1  
	- example: say car [car = 1] say wallet [wallet = 1] say car [car = 2]
	- find keyword in model list
	- find color in model list
	- find size in model list
	- *keyword, color, size [add color and size if we have]
	- sort product by argument
	- get target product then recommend simillar product.	

- Model from OMG title + description
- ID, DESCRIPTION
	(1) Title - Description
	(2) Ttitle - Description
- app.run recommend(item id, number of recommend)
- return similar product with similarly score exmp: 1 05, 2 03, 3 01collections
