# Bird-Images-Search-Engine
The full documentation can be found [here](https://github.com/danielecioffo/Bird-Images-Search-Engine/blob/main/Bird%20Images%20Search%20Engine.pdf). 
The purpose of this project is to create a search engine that can recognize the species of a bird from an image uploaded by the user, proposing also similar pictures. To this end, the following steps were performed.

First of all, our own version of the PP-Index was implemented in order to enable fast similarity search on deep features. In fact, both the images within the database and the user’s queries are represented by feature vectors extracted by means of a Deep Neural Network, so that the similarity between them can be easily computed via a metric such as the Euclidean distance or the cosine similarity. As far as the Deep Neural Network is concerned, ResNet was used as the base architecture, first exploiting feature extraction, and then performing fine tuning of some layers.

Next, the retrieval performance of the image search engine was measured in both the feature extraction and fine-tuning cases, considering various metrics. Furthermore, a brief analysis was performed on the errors made by the system, including a focus on CNN’s explainability. 

Finally, a web user interface was built to allow the search engine to be used from a web browser.
The whole project was developed directly on Google Drive and only later was uploaded to GitHub.
