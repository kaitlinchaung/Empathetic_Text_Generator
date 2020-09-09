# Classifiying Movie Genres from Scripts

***

## Objective

Movies involve visual and audio elements, but can their genres be predicted from the scripts alone?

***

## Methods

The original movie data set had over 400 unique genre combinations, that were subsequently collapsed down 8 classification genres.

In order to represent each script numerically, doc2vec vectors of length=300 were created for each movie script. Additional features aimed to capture how the movie script changes over time. These features included the cosine similarity of the first third and last third of the script, as well as how the sentiment changes over the same time period

*** 

## Takeaways

The best model for this data set with Random Forest, with a F1 score of 0.72.

This model performed the best on the genres of Action Drama and Comedy Drama, with the most misclassifications in Action and Drama. This suggests that there is further work to do in the genre collapsing, as there is likely some redunancy in the classes.
(base) macbook-pro-145:Project_2 kaitlin$ cat ../Project_4
cat: ../Project_4: Is a directory
(base) macbook-pro-145:Project_2 kaitlin$ cat ../Project_4/README.md 
# Generating Empathetic Dialogues

***
 
## Objective

How can we teach a machine to be a more empathetic conversationalist? Can this be used to teach people to be more empathetic?

***

## Methods 

BERT was used to create a sentiment classifer, with a final F1 score of 0.56. LDA was then used to create a topic model of the input prompts and responses.

These 2 tools were used in tandem in order generate a response that contained the same topic and sentiment of the prompt. For each prompt, prompts and responses fitting this criteria were used as the input corpus of the text generator. 

Between a simple Markov model and GPT-2, GPT-2 performed the best in generating more realistic and empathetic responses.

## Data

[Empathetic Dialogues](https://github.com/facebookresearch/EmpatheticDialogues)
