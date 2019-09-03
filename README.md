# Find Donors for CharityML (Supervised Learning)

## Project Overview

CharityML is a fictitious charity organization located in the heart of Silicon Valley that was established to provide financial support for people eager to learn machine learning. After nearly 32,000 letters were sent to people in the community, CharityML determined that every donation they received came from someone that was making more than $50,000 annually. To expand their potential donor base, CharityML has decided to send letters to residents of California, but to only those most likely to donate to the charity. With nearly 15 million working Californians, CharityML would like to build an algorithm to best identify potential donors and reduce overhead cost of sending mail.

The goal of this project is to apply supervised learning techniques and help CharityML identify people most likely to donate to their cause. I evaluated and optimized several different supervised learners to determine which algorithm provided the highest donation yield while also reduced the total number of letters being sent.  Below are the steps, which is documented in [finding_donors.ipynb](https://github.com/iDataist/Find-Donors-for-CharityML/blob/master/finding_donors.ipynb). [visuals.py](https://github.com/iDataist/Find-Donors-for-CharityML/blob/master/visuals.py) provides supplementary visualizations.

- Explored the data to learn how the census data was recorded
- Applied a series of transformations and preprocessing techniques to manipulate the data into a workable format
- Evaluated several supervised learners on the data, and considered which was best suited for the solution
- Optimized the model selected and presented it as the solution to CharityML
- Explored the chosen model and its predictions under the hood, to see just how well it was performing considering the data given

## Project Highlights

This project involved many supervised learning algorithms available in sklearn, and also a method of evaluating just how each model works and performs on a certain type of data. It is important in machine learning to understand exactly when and where a certain algorithm should be used, and when one should be avoided. Below are the key skills demonstrated in the project:

- Identify when preprocessing is needed, and how to apply it
- Establish a benchmark for a solution to the problem
- Evaluate what each of several supervised learning algorithms accomplishes given a specific dataset
- Investigate whether a candidate solution model is adequate for the problem

## Data

The [modified census dataset](https://github.com/iDataist/Find-Donors-for-CharityML/blob/master/census.csv) consists of approximately 32,000 data points, with each datapoint having 13 features. This dataset is a modified version of the dataset published in the paper *"Scaling Up the Accuracy of Naive-Bayes Classifiers: a Decision-Tree Hybrid",* by Ron Kohavi. This paper can be found [online](https://www.aaai.org/Papers/KDD/1996/KDD96-033.pdf), with the original dataset hosted on [UCI](https://archive.ics.uci.edu/ml/datasets/Census+Income).

**Features**
- `age`: Age
- `workclass`: Working Class (Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked)
- `education_level`: Level of Education (Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool)
- `education-num`: Number of educational years completed
- `marital-status`: Marital status (Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse)
- `occupation`: Work Occupation (Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces)
- `relationship`: Relationship Status (Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried)
- `race`: Race (White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black)
- `sex`: Sex (Female, Male)
- `capital-gain`: Monetary Capital Gains
- `capital-loss`: Monetary Capital Losses
- `hours-per-week`: Average Hours Per Week Worked
- `native-country`: Native Country (United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands)

**Target Variable**
- `income`: Income Class (<=50K, >50K)
