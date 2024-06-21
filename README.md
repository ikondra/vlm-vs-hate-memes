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

## Chain-of-Thought 5 - CoT_race5

***Prompt***    
This is an image that may contain hateful content, which is defined as: hatred, hostility, or violence towards member(s) of a race, ethnicity, nation, religion, gender, gender identity, sexual orientation or any other designated sector of society. It may or may not fit the hate category “racism”. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:   
Q1a. Is text present?   
Q1b. What does the text say?    
Q1c. Does the text contain hateful words or phrases?    
Q1d. List all explicit or implied meanings for any hateful words or phrases.    
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?        
Q2c. Does the image contain any hateful visuals?    
Q2d. List all explicit or implied meanings for any hateful visuals.     
Q3. List all explicit or implied meanings of the image and the overlaid text.    
Q4. Is any previously-identified content (particularly humor or sarcasm) directed at specific groups or individuals?    
Q5. Should this image with its overlaid text be considered racism hate? Explain your reasoning. 

## Chain-of-Thought 6 - CoT_race6

***Prompt***    
This is an image that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:   
Q1a. Is text present?   
Q1b. What does the text say?    
Q1c. Does the text contain hateful words or phrases?    
Q1d. List all explicit or implied meanings for any hateful words or phrases.    
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?    
Q2c. Does the image contain any hateful visuals?    
Q2d. List all explicit or implied meanings for any hateful visuals.     
Q3a. Considering the meanings of the overlaid text and the image, list all explicit or implied meanings of the whole input.     
Q3b. Do any of these meanings involve humor or sarcasm?     
Q3c. Is any humor or sarcasm directed at specific groups or individuals?    
Q3d. Is the humor or sarcasm derogatory, demeaning, or otherwise offensive? 
Q4. Should this image with its overlaid text be considered racism hate? Explain your reasoning. 

## Chain-of-Thought 7 - CoT_race7

***Prompt***    
This is an image that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:   
Q1a. Is text present?   
Q1b. What does the text say?    
Q1c. Does the text contain hateful words or phrases?    
Q1d. List all explicit or implied meanings for any hateful words or phrases.    
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?    
Q2c. Does the image contain any hateful visuals?    
Q2d. List all explicit or implied meanings for any hateful visuals.     
Q3. Considering the meanings of the overlaid text from Q1d and the image from Q2d, list all explicit or implied meanings of the whole input.    
Q4. Should this image with its overlaid text be considered racism hate? Explain your reasoning. 

## Chain-of-Thought 8 - CoT_race8

***Prompt***    
This is an image that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:   
Q1a. Is overlaid text present?  
Q1b. What does the text say?    
Q1c. Does the text contain racist words or phrases?     
Q1d. List all explicit or implied meanings for any racist words or phrases. Explain your reasoning.     
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?    
Q2c. Does the image contain any racist visuals?     
Q2d. List all explicit or implied meanings for any racist visuals. Explain your reasoning.  
Q3. Considering the meanings of the overlaid text from Q1d and the image from Q2d, list all explicit or implied meanings of the whole input.    
Q4. Is any previously-identified content (particularly humor or sarcasm) directed at specific groups or individuals?    
Q5. Should this image with its overlaid text be considered racism hate? Explain your reasoning. 

## Chain-of-Thought 9 - CoT_race9

***Prompt***    
This is a meme that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:     
Q1a. Is overlaid text present?  
Q1b. What does the text say?    
Q1c. Does the text contain racist words or phrases?     
Q1d. List all explicit or implied meanings for any racist words or phrases. Explain your reasoning.     
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?    
Q2c. Does the image contain any racist visuals?     
Q2d. List all explicit or implied meanings for any racist visuals. Explain your reasoning.  
Q3. How is the image related to the overlaid text? Explain.     
Q4a. What’s the hidden message in this meme that promotes racism?   
Q4b. Does this meme promote racism in an implicit context or an explicit context?   
Q5. Should this image with its overlaid text be considered racism hate? Explain your reasoning. 

## Chain-of-Thought 10 - CoT_race10

***Prompt***    
This is a meme that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:     
Q1a. Does the text contain racist words or phrases?     
Q1b. List all explicit or implied meanings for any racist words or phrases. Explain your reasoning.     
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?    
Q2c. Does the image contain any racist visuals?     
Q2d. List all explicit or implied meanings for any racist visuals. Explain your reasoning.  
Q3. How is the image related to the overlaid text? Explain.     
Q4a. What’s the hidden message in this meme that promotes racism?   
Q4b. Does this meme promote racism in an implicit context or an explicit context?   
Q5. Should this image with its overlaid text be considered racism hate? Explain your reasoning. 

## Chain-of-Thought 11 - CoT_race11

***Prompt***    
This is a meme that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:     
Q1a. Does the text contain racist words or phrases?     
Q1b. List all explicit or implied meanings for any racist words or phrases. Explain your reasoning.     
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?    
Q2c. List all explicit or implied meanings for any racist visuals. Explain your reasoning.  
Q3. How is the image related to the overlaid text? Explain.     
Q4. What’s the hidden message in this meme that promotes racism?    
Q5. Should this image with its overlaid text be considered racism hate? Explain your reasoning. 

## Chain-of-Thought 12 - CoT_race12

***RAG Query on HatReD Dataset Reasonings***     
What are the elements that make a meme hateful?     

***Prompt***    
This is a meme that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:     
Q1a. Does the text contain racist words or phrases?     
Q1b. List all explicit or implied meanings for any racist words or phrases. Explain your reasoning.     
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?    
Q2c. List all explicit or implied meanings for any racist visuals. Explain your reasoning.  
Q3. How is the image related to the overlaid text? Explain.     
Q4. What’s the hidden message in this meme that promotes racism?    
Q5. Should this image with its overlaid text be considered racism hate? Explain your reasoning. 

## Chain-of-Thought 13 - CoT_race13

***Prompt***    
This is a meme that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:     
Q1a. Does the text contain racist words or phrases?     
Q1b. List all explicit or implied meanings for any racist words or phrases. Explain your reasoning.     
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?        
Q2c. List all explicit or implied meanings for any racist visuals. Explain your reasoning.      
Q3. How is the image related to the overlaid text? Explain.     
Q4. What’s the hidden message in this meme that promotes racism?        
Q5. Should this image with its overlaid text be considered racism hate? Explain your reasoning.     

## Chain-of-Thought 14 - CoT_race14

***RAG Query on HatReD Dataset Reasonings***     
What textual and visual elements make a meme hateful?     

***Prompt***    
Use the following contextual knowledge to answer the prompt below: Textual elements that make a meme hateful include insults, vilification, ridicule, mockery, dehumanization, objectification, and incitement of violence towards specific groups or communities. Visual elements such as images or symbols that reinforce negative stereotypes or discriminatory narratives can also contribute to the hateful nature of a meme.  

This is a meme that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:     
Q1a. Does the text contain racist words or phrases?     
Q1b. List all explicit or implied meanings for any racist words or phrases. Explain your reasoning.     
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?        
Q2c. List all explicit or implied meanings for any racist visuals. Explain your reasoning.      
Q3. How is the image related to the overlaid text? Explain.     
Q4. What’s the hidden message in this meme that promotes racism?        
Q5. Should this image with its overlaid text be considered racism hate? Explain your reasoning.     

## Chain-of-Thought 15 - CoT_race15

***RAG Query on HatReD Dataset Reasonings***     
Is this meme hateful?     

***Prompt***    
Use the following contextual knowledge to answer the prompt below: Yes, this meme is hateful.  

This is a meme that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:     
Q1a. Does the text contain racist words or phrases?     
Q1b. List all explicit or implied meanings for any racist words or phrases. Explain your reasoning.     
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?        
Q2c. List all explicit or implied meanings for any racist visuals. Explain your reasoning.      
Q3. How is the image related to the overlaid text? Explain.     
Q4. What’s the hidden message in this meme that promotes racism?        
Q5. Should this image with its overlaid text be considered racism hate? Explain your reasoning.     

## Chain-of-Thought 16 - CoT_race16

***RAG Query on HatReD Dataset Reasonings***     
What textual and visual elements make a meme hateful?       

***Prompt***        
Use the following contextual knowledge to answer the prompt below: The textual and visual elements that make a meme hateful include derogatory language or stereotypes targeting specific groups of people based on their race, religion, gender, or sexual orientation. Additionally, the visual elements may include images or symbols that reinforce these negative stereotypes or messages, further amplifying the hateful nature of the meme.      

This is a meme that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:     
Q1a. Does the text contain racist words or phrases?     
Q1b. List all explicit or implied meanings for any racist words or phrases. Explain your reasoning.     
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?        
Q2c. List all explicit or implied meanings for any racist visuals. Explain your reasoning.      
Q3. How is the image related to the overlaid text? Explain.     
Q4. What’s the hidden message in this meme that promotes racism?        
Q5. Should this image with its overlaid text be considered racism hate? Explain your reasoning.     

## Chain-of-Thought 17 - CoT_race17

***RAG Query on HatReD Dataset Reasonings***     
What textual and visual elements make a meme hateful?       

***Prompt***        
Use the following contextual knowledge to answer the prompt below: Textual elements that make a meme hateful include insults, vilification, ridicule, objectification, dehumanization, and incitement of violence towards specific groups such as Muslims, Jews, Blacks, LGBT community, females, whites, people of color, and individuals with physical or intellectual disabilities. These elements are conveyed through derogatory statements, stereotypes, and discriminatory remarks targeting the mentioned groups.

Visual elements in hateful memes often accompany the text to reinforce the negative message. These visuals may include offensive imagery, symbols, or illustrations that further degrade or mock the targeted groups. The combination of derogatory text and visuals intensifies the impact of the hateful message, contributing to the harmful nature of the meme.      

This is a meme that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:     
Q1a. Does the text contain racist words or phrases?     
Q1b. List all explicit or implied meanings for any racist words or phrases. Explain your reasoning.     
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?        
Q2c. List all explicit or implied meanings for any racist visuals. Explain your reasoning.      
Q3. How is the image related to the overlaid text? Explain.     
Q4. What’s the hidden message in this meme that promotes racism?        
Q5. Should this image with its overlaid text be considered racism hate? Explain your reasoning.     

## Chain-of-Thought 18 - CoT_race18

***RAG Query on HatReD Dataset Reasonings***     
What specific elements make a meme hateful? Give detailed descriptions and analysis.       

***Prompt***        
Use the following contextual knowledge to answer the prompt below: A meme can be considered hateful based on several specific elements present in its content. These elements include ridiculing or mocking specific groups of people based on their race, ethnicity, religion, gender, or other characteristics. Hateful memes often dehumanize individuals by portraying them as inferior, dangerous, or undesirable. They may also contain derogatory language, stereotypes, or false information intended to incite hatred or violence towards a particular group. Additionally, hateful memes may target vulnerable populations and perpetuate harmful narratives that reinforce discrimination and prejudice. Overall, the key elements that make a meme hateful are the intent to harm, spread negativity, and promote harmful attitudes towards marginalized communities.       

This is a meme that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:     
Q1a. Does the text contain racist words or phrases?     
Q1b. List all explicit or implied meanings for any racist words or phrases. Explain your reasoning.     
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?        
Q2c. List all explicit or implied meanings for any racist visuals. Explain your reasoning.      
Q3. How is the image related to the overlaid text? Explain.     
Q4. What’s the hidden message in this meme that promotes racism?        
Q5. Should this image with its overlaid text be considered racism hate? Explain your reasoning.     

## Chain-of-Thought 19 - CoT_race19

***RAG Query on HatReD Dataset Reasonings***     
What specific textual and visual elements make a meme hateful?       

***Prompt***        
Use the following contextual knowledge to answer the prompt below: Specific textual elements that make a meme hateful include insults, vilification, ridicule, objectification, dehumanization, and incitement of violence. Visual elements such as images or symbols that reinforce these negative messages can also contribute to the hateful nature of a meme.       

This is a meme that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:     
Q1a. Does the text contain racist words or phrases?     
Q1b. List all explicit or implied meanings for any racist words or phrases. Explain your reasoning.     
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?        
Q2c. List all explicit or implied meanings for any racist visuals. Explain your reasoning.      
Q3. How is the image related to the overlaid text? Explain.     
Q4. What’s the hidden message in this meme that promotes racism?        
Q5. Should this image with its overlaid text be considered racism hate? Explain your reasoning.     

## Chain-of-Thought 20 - CoT_race20

***RAG Query on HatReD Dataset Reasonings***     
What specific textual and visual elements make a meme hateful?       

***Prompt***        
Use the following contextual knowledge to answer the prompt below: The specific textual and visual elements that make a meme hateful include ridiculing or insulting specific groups of people based on their race, religion, or sexual orientation. This can be achieved through mocking stereotypes, making derogatory remarks, or dehumanizing individuals. Additionally, the use of offensive language, derogatory imagery, and promoting violence or discrimination towards a particular group can also contribute to the hateful nature of a meme.The specific textual and visual elements that make a meme hateful include ridiculing or insulting specific groups of people based on their race, religion, or sexual orientation. This can be achieved through mocking stereotypes, making derogatory remarks, or dehumanizing individuals. Additionally, the use of offensive language, derogatory imagery, and promoting violence or discrimination towards a particular group can also contribute to the hateful nature of a meme.       

This is a meme that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:     
Q1a. Does the text contain racist words or phrases?     
Q1b. List all explicit or implied meanings for any racist words or phrases. Explain your reasoning.     
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?        
Q2c. List all explicit or implied meanings for any racist visuals. Explain your reasoning.      
Q3. How is the image related to the overlaid text? Explain.     
Q4. What’s the hidden message in this meme that promotes racism?        
Q5. Should this image with its overlaid text be considered racism hate? Explain your reasoning.     

## Chain-of-Thought 21 - CoT_race21

***RAG Query on HatReD Dataset Reasonings***     
What specific textual and visual elements make a meme hateful?       

***Prompt***        
Use the following contextual knowledge to answer the prompt below: The specific textual and visual elements that make a meme hateful include ridiculing, insulting, vilifying, objectifying, dehumanizing, mocking, and inciting violence against specific groups or communities based on their race, religion, gender, or other characteristics. This can be achieved through derogatory language, stereotypes, false accusations, and harmful imagery that target and demean these groups.       

This is a meme that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:     
Q1a. Does the text contain racist words or phrases?     
Q1b. List all explicit or implied meanings for any racist words or phrases. Explain your reasoning.     
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?        
Q2c. List all explicit or implied meanings for any racist visuals. Explain your reasoning.      
Q3. How is the image related to the overlaid text? Explain.     
Q4. What’s the hidden message in this meme that promotes racism?        
Q5. Should this image with its overlaid text be considered racism hate? Explain your reasoning.     

## Chain-of-Thought 22 - CoT_race22

***RAG Query on HatReD Dataset Reasonings***     
What textual and visual elements make a meme hateful?       

***Prompt***        
Use the following contextual knowledge to answer the prompt below: The textual and visual elements that make a meme hateful include derogatory language or stereotypes targeting specific groups of people based on their race, religion, gender, or sexual orientation. The use of mocking, insulting, or dehumanizing language towards these groups, along with the portrayal of negative stereotypes or harmful actions in the visual content, contribute to the hateful nature of the meme.       

This is a meme that may contain racist content. Racism is defined as: actions, biases, prejudices, or beliefs on the part of one group or individual that discriminates against, marginalizes, or in any way oppresses another group or individual that is perceived as being racially different. With this knowledge, please answer the following questions, in order:     
Q1a. Does the text contain racist words or phrases?     
Q1b. List all explicit or implied meanings for any racist words or phrases. Explain your reasoning.     
Q2a. List all components and entities in the image.     
Q2b. What is happening in the image?        
Q2c. List all explicit or implied meanings for any racist visuals. Explain your reasoning.      
Q3. How is the image related to the overlaid text? Explain.     
Q4. What’s the hidden message in this meme that promotes racism?        
Q5. Should this image with its overlaid text be considered racism hate? Explain your reasoning.     

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
