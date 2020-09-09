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
