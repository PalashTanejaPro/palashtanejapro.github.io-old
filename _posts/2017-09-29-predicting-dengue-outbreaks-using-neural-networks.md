---
title: Predicting dengue outbreaks using Neural Networks
---

### Introduction
Dengue fever is a mosquito-borne tropical disease caused by the dengue virus. Symptoms typically begin three to fourteen days after infection. This may include a high fever, headache, vomiting, muscle and joint pains, and a characteristic skin rash. Recovery generally takes two to seven days. In a small proportion of cases, the disease develops into the life-threatening dengue hemorrhagic fever, resulting in bleeding, low levels of blood platelets and blood plasma leakage, or into dengue shock syndrome, where dangerously low blood pressure occurs.

Each year between 50 and 528 million people are infected and approximately 10,000 to 20,000 die due to Dengue Fever.

### Methodology
Research papers predicting dengue generally use meteorological data and don't consider past incidence of the disease, which I found out to be a more important factor than weather conditions. 
>Researchers are not employing deep learning techniques and use simpler regression techniques like linear regression.

I scraped dengue and weather data from the data.gov.sg and compiled it into one clean dataset. Contrary to research papers I used past incidence to predict future incidence. Then I created a neural network with 3 layers which contained 13 nodes each. I used sklearn's train and test split function which split my 277 length dataset into 75% training data and 25% testing data.

### Results
My neural net was able to achieve an **R<sup>2</sup> value of 0.9316** which is much better than the *state-of-the-art* values that other Researchers have got. The **mean error of my model was only 35.11 cases**. This proves that dengue prediction can be done very accurately even if a small dataset is available like the one I used. It also goes to show how deep learning can provide substantially better results even on very small datasets.

<amp-img src="{{site.url}}/assets/images/dengue.png" layout="responsive" alt="Results" height="800" width="1220" ></amp-img>

### Resources
The dataset is free for anyone to use if they give appropriate credit to me.[ Email me for a copy.](mailto:tanejapalash@gmail.com)

*If you would like to have dengue predicted in your area, send me a dataset at my email and I will be happy to run my model on your dataset.*