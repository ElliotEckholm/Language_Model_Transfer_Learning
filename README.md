# Transfer Learning using a Language Model with Fastai

Goal: Predict whether a user will like new articles within a domain based on past likes

## Wikitext Language Model -> NASA Article Title Language Model -> NASA Likes Classification Model

Using Transfer Learning with Language Model Trained on WikiText, then trained on NASA Article Titles (Target Corpus) then transferred to Classification Model to Predict if Title is Liked

## Results

#### True => User will Like
#### False => User will Not Like

* learn.predict("SpaceX Dragon Launched") -> True
* learn.predict("Dark Matter is Discovered") -> True
* learn.predict("Boring Stuff") -> False
* learn.predict("California is seen from Space") -> False
* learn.predict("Apollo 57 Launches for the first time") -> True
* learn.predict("Article Title not related at all") -> False
* learn.predict("Biology is used in space") -> False
* learn.predict("The White House makes mistakes about space") -> False
* learn.predict("Station Crew Sees Typhoon from Space") -> False


## Future Improvements
* Gather more NASA/Space Articles
* Use Article's Descriptions + Title
* Experiment with Models Hyperparameters 
* Increase number of Epochs
