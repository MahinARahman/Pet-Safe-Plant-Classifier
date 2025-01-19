# Pet-Safe-Plant-Classifier
We developed a model that classifies whether houseplants are safe for different pets in US households. 
# Tools and Techniques
Python on Google Colab 
# Dataset
**Houseplant species**
14774 images across 47 classes
Data Source: [Kaggle](https://www.kaggle.com/datasets/kacpergregorowicz/house-plant-species) 

**Pets**
Top 5 pets in US households that can be exposed to plants by [American Veterinary Medical Association](https://www.avma.org/resources-tools/reports-statistics/us-pet-ownership-statistics).
Effects of exposure to toxic house plants by [American Society for the Prevention of Cruelty to Animals](https://www.aspca.org/pet-care/animal-poison-control/toxic-and-non-toxic-plants).

# Modeling 
4 different neural network models were trained and evaluated: 
- ViT pre-trained on ImageNet 
- ViT pre-trained on PlantNet (specialized for plant images)
- Custom ViT trained from scratch on our dataset 
- Custom EfficientNet-B3

ViT Pre-Trained on PlantNet stood out as the most effective model with 92% accuracy and smooth decline of train and test loss curves. 
Pandas Dictionary for mapping top pets in USA households (dogs, cats, rabbits, reptiles and birds) to effects of exposure to house plants was created.

# Results
Model was able to identify image of Hyacinth and highlight the negative impact of this plant on cats, dogs and rabbits upon exposure. We recommend continuously expanding the database to include newer plant species and additional pet categories to maintain the model's robustness and relevance.
