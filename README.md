## General with Context Statement

***Prompt***  
You are a hate speech detection expert system that aims to protect the friendly atmosphere of social networks. Here is one picture. Please judge whether the picture is hateful or not-hateful.

## Chain-of-Thought

***Prompt***  
This is an image that may or may not contain hateful content. Hate is defined as: hatred, hostility, or violence towards member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation or any other designated sector of society.

Please answer the following questions, in order:  
Q1a. Is there any text present in the image?  
Q1b. If the answer to Part A was "yes": Ignoring the image, what does the overlaid text say?  
Q1c. If the answer to Part A "yes": Are there any derogatory, humiliating, insulting, or disparaging words or phrases used?  
Q2a. Ignoring the overlaid text, what does the image depict?  
Q2b. Are there any derogatory, humiliating, insulting, or disparaging components of the image?  
Q2c. Is there any symbolism or imagery used by known hateful groups?  
Q2d. Is there any symbolism or imagery used as a stand-in or reference to any marginalized groups or other designated sectors of society?  
Q3. Taking into account the previous answers, could the text be describing something about the image that makes it hateful in this context?  
Q4. Based on the definition of “hate” as hatred, hostility, or violence towards member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation or any other designated sector of society,  should this image be classified as hateful? Explain your reasoning.  

## In-Context Learning Chain-of-Thought

***Prompt***    
prompt here