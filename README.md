# Project Overview
## Project Aim
This project aims to explore a knowledge graph of skincare products and their constituent active ingredients which highlights the beneficial and adverse interaction effects. This would allow users to understand whether certain skincare products should be used together for added benefits or whether it would be best to avoid using the products at the same time because of possible adverse effects.
The final product looks like this:

 ![final_product](https://github.com/solarspaceclouds/Skincare-Knowledge-Graph/assets/65459827/aceb14ad-0828-4392-aa67-a2170f8d5640)

## Project Significance: Why is this useful?
To help people in their decision-making when planning which products to use in their skincare routine so that they 
1. Know which products to avoid using together because of potential adverse interaction effects among their active ingredients, 
2. Take advantage of any potential beneficial interaction effects between different products which they own to optimise the value of their skincare products.

## Project Motivation/Research Gap:
Currently, skincare brands tend to recommend products of the same brand in order to maximise the business profit. However, in today's world of e-commerce, skincare junkies are spoilt for choice. It is very tempting (and usually satisfying) to purchase and lather on all the skincare products one is attracted to, but at what cost? We have little knowledge and access to information about the compatibility of products from different skincare brands. This thus begs the question: Is using our faces as a testing ground for chemical reactions the only way to find out how different skincare products interact with each other? 

## Project Motivation: Personal Story-time: 
In recent months, I have developed a slight obsession with skincare products while starting my journey on anti-aging. It has been quite a fun ride so far, and although my enthusiastic slathering of various skincare products all over my face in my morning and night routine have gained me some compliments about having glass/glowy skin, there have been one or two instances where I felt a strange prickly sensation on my cheeks which was followed by redness. Lucky for me, it subsided quickly enough after I washed my face (within the morning), but it a little destabilising to experience such an effect - I guess it really hit me then that I've been using my face as a canvas for chemical experiments, and one day my skin won't be thanking me anymore for the way I've been treating it.

## Important Notes/Disclaimers: 
1. This project is mainly meant as a pet project for me to learn how to create a knowledge graph and frame a project idea in a specific industry domain for it. 
2. This project was done without the consultation of skincare professionals/pharmacists/dermatologists. 
3. The information presented by the knowledge graphs have yet to be verified by industry professionals. 
4. The list of active ingredients identified in this project are not exhaustive because it is based on my own basic knowledge and research. All the predefined rules of the interaction effects between different active ingredients are based on a consolidation of information from online articles.

## File Details
1. webscraping_insidecoder.ipynb scrapes the products details and saved in many_products.csv. Product details were scraped according to the brands defined in the 'brands' variable near the beginning of the notebook (after import statements)
   - If you would like to scrape your own data, please modify the 'brands' variable or code as desired and output the desired information as structured in many_products.csv
   - Otherwise, if you would like to jump straight to the knowledge graph, you don't have to explore this notebook and can jump straight to the knowledge_graph_creation.ipynb. (many_products.csv has been included in this repository for reference for this purpose.)  
2. knowledge_graph_creation.ipynb uses the scraped data in many_products.csv to build a finalised knowledge graph. (on http://127.0.0.1:8050/) 
3. web_ui_modifications_variations.ipynb has many variations of the knowledge graph that I tried out in the process of trying to build and settle on the finalised knowledge graph. Feel free to explore these if you are interested. 

## How to use the knowledge graph visualisation:
1. In the search bar, type in the search term (brand name/ingredient name/specific product name). A drop-down list of possible selections will be constantly updated according to your typed input. Select your desired ingredient.
2. Then in the search bar, continue to search and select the next product to see the interaction effects among the products. 

### Product Brands 
In this project, the product and ingredient data were scraped (based on brand name) from the incidecoder.com website, which is a well-known public repository that provides information on skincare products and ingredients. 
The chosen brand names scraped for the purpose of this project were: 

"Kiehl's", "Clarins", "Sulwhasoo", "Hera", "La Mer", "Clinique", "Lancome", "Elizabeth Arden","Skin Inc", "Decorte", "Fresh", "Sk ii", "Sum 37", "Givenchy", "Loreal", "Guerlain","Vichy","The Ordinary"

##  Knowledge Graph Visualisation
2 products with no interaction effects between their active ingredients

![2_products](https://github.com/solarspaceclouds/Skincare-Knowledge-Graph/assets/65459827/3a22da3b-453a-4179-93ce-55dd5941345d)

2 products with beneficial interaction effects between their active ingredients

![2_beneficial_graph](https://github.com/solarspaceclouds/Skincare-Knowledge-Graph/assets/65459827/e1c9764e-5e4b-4a5c-a1bf-6b905d297df8)

2 products with adverse interaction effects between their active ingredients

![2_adverse_graph](https://github.com/solarspaceclouds/Skincare-Knowledge-Graph/assets/65459827/67ac5183-c087-40be-86d0-4f2fa7f157bd)


3 products with both beneficial and adverse interaction effects among their active ingredients

 ![3_beneficial_adverse_pic](https://github.com/solarspaceclouds/Skincare-Knowledge-Graph/assets/65459827/e9e21f3c-a9da-4d2f-8e71-2f964936cce5)


### Additional notes: 
- This skincare knowledge graph is not deployed and is only for personal use/research purposes because of the lack of verification of correctness of the displayed information as explained in the Important Notes/Disclaimers section above.
- Initially, I planned to obtain active ingredients interaction information via extracting insights from the transcripts of the videos made by the popular dermatologist youtube channel: Doctorly. However, this endeavour which involved various steps such as transcript scraping, named entity recognition and (active ingredients interaction effects) insights extraction proved to be fairly challenging. It posed a significant distraction to the main focus of this project, which was to understand how to create a knowledge graph. Hence, I settled on the method of gathering information from online articles to identify the active ingredients and draft up predefined interaction rules to the best of my knowledge and understanding. In future, it would be beneficial to verify the information in this portion.

For more detailed explanation, check out the Medium article coming soon!
