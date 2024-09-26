# Clean-Cyber-Bullying-Tweet-Analysis

# Data Source:
The dataset contains 47,692 tweets categorized into six classes: Age, Ethnicity, Gender, Religion, Other Cyberbullying, and Not Cyberbullying.

# Workflow:
## Raw Data Processing:

Tweets were cleaned through various steps, including lemmatization, removal of stopwords, regex substitution, lowercasing, and tokenization.
Data was split into training and validation sets using one-hot encoding.
## Exploratory Data Analysis:

Word clouds and visual representations were created to explore the distribution of words across categories.
Correlation analysis was performed to understand the key patterns.
## Text Modeling:

Three models were tested: ERNIE, XLNet, and RoBERTa.
These models used tokenization and were optimized using techniques like early stopping, learning rate reduction, and checkpointing.
## Model Evaluation:

RoBERTa achieved the highest accuracy of 85.98% with strong precision and recall.
Overfitting was observed across models, as training accuracy exceeded validation accuracy. Techniques like regularization and dropout were recommended to mitigate this.
## Key Findings:
RoBERTa was the best-performing model, with a validation accuracy of 85.98%.
The model struggled to distinguish between Not Cyberbullying and other categories, especially in terms of recall for the Not Cyberbullying class.
To improve the models, further regularization, dropout layers, and hyperparameter tuning are suggested.
