* Collaborative filtering: Recommend to target user items that other similar users liked in the past
* Content-based filtering: Recommend to target user content similar to what he or she liked in the past
* Context-aware recommender system: Recommend to target user items that he, she, or other users liked in a given context or situation
* Hybird RS: Any combination of the above

# Problems
* Cold-start problems (new users/items unknown to the system)
* Privacy and security concerns
* Lack of transparency and explainability
* Over-personalizaation -> filter bubble
* Different user intents, exploration vs exploitation
* Biases
* Fairness & Discrimination

# Biases in Recommendations
* Data unbalanced
* Algorithms, reinforcing stereotypes or amplfy alread popular content
* Presentation
* User cognition, perception
Popularity bias:
* reinforcing already popular items/artists, while limiting exposure of less popular ones

## Mitigation
* Pre-processing: Data rebalancing, e.g. upsample minarity group
* In-processing: Adverarial training, train classifier that predicts the prodected user attribute
* Post-processing: Reweigh/rank items in recommendation list