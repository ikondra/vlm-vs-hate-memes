# Prompts

## General with Context Statement - context_general

***Prompt***  
You are a hate speech detection expert system that aims to protect the friendly atmosphere of social networks. Here is one picture. Please judge whether the picture is hateful or not-hateful.

## Chain-of-Thought 0 - CoT

***Prompt***  
This is an image that may or may not contain hateful content. Hate is defined as: hatred, hostility, or violence towards member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation or any other designated sector of society.

Please answer the following questions, in order:  
Q1a. Is there any text present in the image?  
Q1b. If the answer to Part A was "yes": Ignoring the image, what does the overlaid text say?  
Q1c. If the answer to Part A was "yes": Are there any derogatory, humiliating, insulting, or disparaging words or phrases used?  
Q2a. Ignoring the overlaid text, what does the image depict?  
Q2b. Are there any derogatory, humiliating, insulting, or disparaging components of the image?  
Q2c. Is there any symbolism or imagery used by known hateful groups?  
Q2d. Is there any symbolism or imagery used as a stand-in or reference to any marginalized groups or other designated sectors of society?  
Q3. Taking into account the previous answers, could the text be describing something about the image that makes it hateful in this context?  
Q4. Based on the definition of “hate” as hatred, hostility, or violence towards member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation or any other designated sector of society,  should this image be classified as hateful? Explain your reasoning.  

## Chain-of-Thought 1 - CoT1

***Prompt***  
This is an image that may or may not contain hateful content.  

Please answer the following questions, in order:  
Q1a. Is there any text present in the image?  
Q1b. Ignoring the image, what does the overlaid text say?  
Q1c. Are there any derogatory, humiliating, insulting, or disparaging words or phrases used?  
Q1d. Are any hateful or offensive components directed at specific groups or individuals?  
Q2a. Ignoring the overlaid text, what does the image depict?  
Q2b. Are there any hateful or offensive components of the image?  
Q2c. Is there any symbolism or imagery used as a reference to any specific groups or individuals?  
Q2d. Are any hateful or offensive components directed at specific groups or individuals?  
Q3. Considering all previous answers, is the text describing something about the image that makes it hateful in this context?  
Q4. Based on the definition of “hate” as hatred, hostility, or violence towards member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation or any other designated sector of society, should this image be classified as hateful? Explain your reasoning.  

## Chain-of-Abstraction 0 - CoT_race0

***Prompt***    
This is an image that may or may not contain hateful content that fits the hate category _{category}_. Please answer the following questions, in order:   
Q1a. Is there any text present in the image?    
Q1b. Ignoring the image, what does the overlaid text say?   
Q1c. Are there any derogatory, humiliating, insulting, or disparaging words or phrases used that fit the hate category _{category}_?  
Q1d. Are any hateful or offensive components identified in Q1c directed at specific groups or individuals?
Q2a. Ignoring the overlaid text, what does the image depict?    
Q2b. Are there any hateful or offensive components of the image that fit the hate category _{category}_?  
Q2c. Is there any symbolism or imagery used as a reference to any specific groups or individuals?   
Q2d. Are any of the hateful or offensive components identified in Q2b directed at specific groups or individuals?   
Q3. Considering all previous answers, is the text describing something about the image that makes it hateful under the category of _{category}_ in this context?  
Q4. Based on the definition of “_{category}_” as _{definition}_, should this image be classified as _{category}_ hate? Explain your reasoning.    

## Chain-of-Abstraction 1 - CoT_race1

***Prompt***
This is an image that may or may not contain hateful content, which is defined as hatred, hostility, or violence towards member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation or any other designated sector of society. It may or may not fit the hate category “_{category}_”, which is defined as _{definition}_. Please answer the following questions, in order:
Q1a. Is there any text present in the image?
Q1b. Ignoring the image, what does the overlaid text say?
Q1c. Are there any derogatory, humiliating, insulting, or disparaging words or phrases used that fit the hate category “_{category}_”?
Q1d. Are any hateful or offensive components identified in Q1c directed at specific groups, cultures, or individuals?
Q2a. Ignoring the overlaid text, what does the image depict?
Q2b. Is there any symbolism or imagery used as a reference to any specific groups, cultures, or individuals?
Q2c. Are any of the hateful or offensive components identified in Q2b directed at specific groups or individuals?
Q3. Considering all previous answers, is the text describing something about the image that makes it hateful under the category of “_{category}_” in this context?
Q4. Based on the definition of “_{category}_” as _{definition}_, should this image be classified as _{category}_ hate? Explain your reasoning.

## Chain-of-Thought 2 - CoT_race2

***Prompt***    
This is an image that may or may not contain hateful content, which is defined as hatred, hostility, or violence towards member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation or any other designated sector of society. It may or may not fit the hate category “racism”, which is defined as policies, behaviors, rules, etc. that result in a continued unfair advantage to some people and unfair or harmful treatment of others based on race. Please answer the following questions, in order:   
Q1a. Is there any text present in the image?    
Q1b. Ignoring the image, what does the overlaid text say?   
Q1c. Are any racist words or phrases (or similarly derogatory, humiliating, insulting, or disparaging words or phrases) used?   
Q1d. Are any words or phrases identified in Q1c directed at specific groups, cultures, or individuals?  
Q2a. Ignoring the overlaid text, list all of the components of the image.   
Q2b. Are any words or phrases identified in the overlaid text directed towards any of the image components identified in Q2a?   
Q3a. Considering all previous answers, does any element of the overlaid text recontextualize any image components into racist hate? 
Q3b. Considering all previous answers, do any image components recontextualize any elements of the overlaid text into racist hate?  
Q4. Based on the definition of “racism” as policies, behaviors, rules, etc. that result in a continued unfair advantage to some people and unfair or harmful treatment of others based on race, should this image be classified as racism hate? Consider all previous answers, and explain your reasoning.  

## Chain-of-Thought 3 - CoT_race3

***Prompt***    
This is an image that may or may not contain hateful content, which is defined as hatred, hostility, or violence towards member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation or any other designated sector of society. It may or may not fit the hate category “racism”. Racism is defined as actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With the above knowledge, please answer the following questions, in order: 
Q1a. Is there any text present in the image?    
Q1b. Ignoring the image, what does the overlaid text say?   
Q1c. Are any racist words or phrases (or similarly derogatory, humiliating, insulting, or disparaging words or phrases) used?   
Q1d. Are any words or phrases identified in Q1c directed at specific groups, cultures, or individuals? Answer in the following format: use of derogatory terms against {target} {predicate}, where {target} represents the attacked social target and {predicate} highlights the hateful implication.   
Q2a. Ignoring the overlaid text, list all of the components of the image.   
Q2b. Are any words or phrases identified in the overlaid text directed towards any of the image components identified in Q2a? Answer in the following format: use of derogatory terms against {target} {predicate}, where {target} represents the attacked social target and {predicate} highlights the hateful implication.    
Q3a. Considering all previous answers, does any element of the overlaid text recontextualize any image components into racist hate? 
Q3b. Considering all previous answers, do any image components recontextualize any elements of the overlaid text into racist hate?  
Q4. Based on the definition of racism, should this image be classified as racism hate? Consider all previous answers, and explain your reasoning.   

## Chain-of-Thought 4 - CoT_race4

***Prompt***
This is an image that may contain hateful content, which is defined as hatred, hostility, or violence towards member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation or any other designated sector of society. It may or may not fit the hate category “racism”. Racism is defined as actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With the above knowledge, please answer the following questions, in order:    
Q1. List all explicit or implied meanings of the image and the overlaid text.   
Q2. Is there any content (particularly humor or sarcasm) identified in Q1 directed at specific groups or individuals?   
Q3. Should this image with its overlaid text be considered racism hate? Explain your reasoning. 

## In-Context Learning Chain-of-Thought - in_context_learning_CoT

***Prompt***    
These images may or may not contain hateful content. Hate is defined as: hatred, hostility, or violence towards member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation or any other designated sector of society. Images #1 through #4 and the associated questions and answers are provided as examples.  

![img1](https://github.com/ikondra/vlm-vs-hate-memes/assets/56898088/0b59ce81-10a8-4a36-b014-0c88eebecb57)  
The following questions and answers are for Image #1:  
Q1a. Is there any text present in the image?  
A: Yes, there is text present in the image.  
Q1b. If the answer to Part A was "yes": Ignoring the image, what does the overlaid text say?  
A: The overlaid text says "when you get to choose your own mental illness."  
Q1c. If the answer to Part A "yes": Are there any derogatory, humiliating, insulting, or disparaging words or phrases used?  
A: The phrase "choose your own mental illness" could be considered disparaging or insulting as it implies mental illness is a choice, which is a mischaracterization and could be offensive to those with mental health issues.  
Q2a. Ignoring the overlaid text, what does the image depict?  
A: The image depicts a hand with a thumb up, stylized in the colors of the rainbow, which is commonly associated with the LGBTQ+ community.  
Q2b. Are there any derogatory, humiliating, insulting, or disparaging components of the image?  
A: There are no overtly derogatory, humiliating, insulting, or disparaging components in the illustration of the hand.  
Q2c. Is there any symbolism or imagery used by known hateful groups?  
A: There is no overt symbolism or imagery used by known hateful groups.  
Q2d. Is there any symbolism or imagery used as a stand-in or reference to any marginalized groups or other designated sectors of society?  
A: The rainbow coloring of the thumb is a known symbol for LGBTQ+ pride and can be a reference to this marginalized group.  
Q3. Taking into account the previous answers, could the text be describing something about the image that makes it hateful in this context?  
A: The text could be interpreted as making a negative statement about the LGBTQ+ community by implying that being a part of this community or its associated identities is akin to choosing a mental illness. This can be seen as a disparaging connection between LGBTQ+ identities and mental illness.  
Q4. Based on the definition of “hate” as hatred, hostility, or violence towards member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation or any other designated sector of society, should this image be classified as hateful? Explain your reasoning.  
A: Based on the combination of the text and the image, this content should be classified as hateful. It juxtaposes a recognized symbol of LGBTQ+ pride with text that suggests a negative and false narrative about mental illness, which could be seen as promoting hostility towards the LGBTQ+ community. This message may perpetuate harmful stereotypes and contribute to the discrimination and stigmatization of LGBTQ+ individuals. Therefore, it could be considered hostile towards a specific sector of society based on sexual orientation and gender identity.  

![img2](https://github.com/ikondra/vlm-vs-hate-memes/assets/56898088/a00f9f3c-19a5-433a-b28b-1138490b8311)   
The following questions and answers are for Image #2:  
Q1a. Is there any text present in the image?  
A: Yes, there is text present in the image.  
Q1b. If the answer to Part A was "yes": Ignoring the image, what does the overlaid text say?  
A: The text says "when you have an 80 point iq but it's the highest in your village"  
Q1c. If the answer to Part A "yes": Are there any derogatory, humiliating, insulting, or disparaging words or phrases used?  
A: The text includes a sarcastic remark possibly intended to denigrate the intellectual capacity of an individual or group and could be considered disparaging.  
Q2a. Ignoring the overlaid text, what does the image depict?  
A: The image depicts a person who appears to be of African descent looking directly at the camera with a neutral or possibly unimpressed expression on their face.  
Q2b. Are there any derogatory, humiliating, insulting, or disparaging components of the image?  
A: There are no overtly derogatory, humiliating, insulting, or disparaging components present in the image of the person itself.  
Q2c. Is there any symbolism or imagery used by known hateful groups?  
A: There is no apparent symbolism or imagery used by known hateful groups in the image.  
Q2d. Is there any symbolism or imagery used as a stand-in or reference to any marginalized groups or other designated sectors of society?  
A: There is no apparent symbolism or imagery used as a stand-in or reference to any marginalized groups or other designated sectors of society in the image itself.  
Q3. Taking into account the previous answers, could the text be describing something about the image that makes it hateful in this context?  
A: Yes, in the context of the text describing an individual with an "80 point iq," it associates the person in the image with this description, which could be interpreted as mocking or devaluing the intelligence of someone.  
Q4. Based on the definition of “hate” as hatred, hostility, or violence towards member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation or any other designated sector of society, should this image be classified as hateful? Explain your reasoning.  
A: The image, coupled with the text, seems to ridicule the person based on perceived low intelligence. While this does not target a specific member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation, or any other designated sector of society, it could be seen as spreading negativity or promoting stereotypes against individuals based on intellect, which can be considered a form of hate under a broader interpretation of the definition. Thus, some might classify this image as hateful due to its derogatory and mocking nature, while others might see it as a distasteful joke not specifically targeting any protected group.  

![img3](https://github.com/ikondra/vlm-vs-hate-memes/assets/56898088/bfb21e20-3ef5-4999-9f17-8071a23f45ee)  
The following questions and answers are for Image #3:  
Q1a. Is there any text present in the image?  
A: Yes, there is text present in the image.  
Q1b. If the answer to Part A was "yes": Ignoring the image, what does the overlaid text say?  
A: The overlaid text says "when is the time to eat i am hungry."  
Q1c. If the answer to Part A "yes": Are there any derogatory, humiliating, insulting, or disparaging words or phrases used?  
A: No, there are no derogatory, humiliating, insulting, or disparaging words or phrases used in the text.
Q2a. Ignoring the overlaid text, what does the image depict?  
A: Ignoring the overlaid text, the image depicts a pig looking towards what appears to be a feeding trough.  
Q2b. Are there any derogatory, humiliating, insulting, or disparaging components of the image?  
A: There are no derogatory, humiliating, insulting, or disparaging components visible in the image itself.  
Q2c. Is there any symbolism or imagery used by known hateful groups?  
A: There is no symbolism or imagery used by known hateful groups in the image.  
Q2d. Is there any symbolism or imagery used as a stand-in or reference to any marginalized groups or other designated sectors of society?  
A: There is no symbolism or imagery used as a stand-in or reference to any marginalized groups or other designated sectors of society in the image.  
Q3. Taking into account the previous answers, could the text be describing something about the image that makes it hateful in this context?  
A: The text does not describe anything about the image that makes it hateful in this context. It appears to be a humorous or whimsical caption representing what the pig might be thinking.  
Q4. Based on the definition of “hate” as hatred, hostility, or violence towards member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation or any other designated sector of society, should this image be classified as hateful? Explain your reasoning.  
A: Based on the definition of “hate” provided, this image should not be classified as hateful. It simply shows a pig with text that anthropomorphizes it with a common desire to eat when hungry. There is no indication of hatred, hostility, or violence towards any group of society.  

![img4](https://github.com/ikondra/vlm-vs-hate-memes/assets/56898088/39f0972b-a029-4480-975e-d4a6af35d74a)  
The following questions and answers are for Image #4:  
Q1a. Is there any text present in the image?  
A: Yes, there is text present in the image.  
Q1b. If the answer to Part A was "yes": Ignoring the image, what does the overlaid text say?  
A: The overlaid text says "all you guys think about is dope".  
Q1c. If the answer to Part A "yes": Are there any derogatory, humiliating, insulting, or disparaging words or phrases used?  
A: No, there are no derogatory, humiliating, insulting, or disparaging words or phrases used in the text itself.
Q2a. Ignoring the overlaid text, what does the image depict?  
A: The image depicts a person with a stern expression, wearing a bow tie, suspenders, and glasses.  
Q2b. Are there any derogatory, humiliating, insulting, or disparaging components of the image?  
A: There are no inherently derogatory, humiliating, insulting, or disparaging components of the image of the person itself.  
Q2c. Is there any symbolism or imagery used by known hateful groups?  
A: There is no obvious symbolism or imagery used by known hateful groups in the image.  
Q2d. Is there any symbolism or imagery used as a stand-in or reference to any marginalized groups or other designated sectors of society?  
A: There is no apparent symbolism or imagery used as a stand-in or reference to any marginalized groups or other designated sectors of society in the image.  
Q3. Taking into account the previous answers, could the text be describing something about the image that makes it hateful in this context?  
A: The text does not appear to describe anything about the image that makes it hateful in the given context. The text seems to be a general statement without targeting any specific group or individual.  
Q4. Based on the definition of “hate” as hatred, hostility, or violence towards member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation or any other designated sector of society, should this image be classified as hateful? Explain your reasoning.  
A: Based on the provided definition of “hate” and the analysis above, this image should not be classified as hateful. The text and the image, when taken together, do not express hatred, hostility, or violence towards any members of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation, or any other designated sector of society. It appears to be a statement that could be interpreted in various non-hateful ways.  

Please answer the following questions, in order, about image #5:  
Q1a. Is there any text present in the image?  
Q1b. If the answer to Part A was "yes": Ignoring the image, what does the overlaid text say?  
Q1c. If the answer to Part A "yes": Are there any derogatory, humiliating, insulting, or disparaging words or phrases used?  
Q2a. Ignoring the overlaid text, what does the image depict?  
Q2b. Are there any derogatory, humiliating, insulting, or disparaging components of the image?  
Q2c. Is there any symbolism or imagery used by known hateful groups?  
Q2d. Is there any symbolism or imagery used as a stand-in or reference to any marginalized groups or other designated sectors of society?  
Q3. Taking into account the previous answers, could the text be describing something about the image that makes it hateful in this context?  
Q4. Based on the definition of “hate” as hatred, hostility, or violence towards member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation or any other designated sector of society,  should this image be classified as hateful? Explain your reasoning.  
