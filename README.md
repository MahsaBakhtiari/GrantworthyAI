![](https://sos-ch-dk-2.exo.io/public-website-production-2022/filer_public_thumbnails/filer_public/72/b7/72b7892e-4826-4a92-848d-9d9fcdfb0768/hbp_team_proposes_new_categorisation_scheme_for_neuron-astrocyte_network_models-1.png__945x706_q85_subsampling-2.png)
# GrantworthyAI
## This repository is a project aimed at developing a deep learning neural network model that assists AlphabetSoup in identifying and choosing funding applicants who are most likely to succeed in their entrepreneurial endeavors.

### The project has two main parts:

#### 1. Preprocess the Data
- Within this dataset are a number of columns that capture metadata about each organization, such as:
    * EIN and NAME—Identification columns
    * APPLICATION_TYPE—Alphabet Soup application type
    * AFFILIATION—Affiliated sector of industry
    * CLASSIFICATION—Government organization classification
    * USE_CASE—Use case for funding
    * ORGANIZATION—Organization type
    * STATUS—Active status
    * INCOME_AMT—Income classification
    * SPECIAL_CONSIDERATIONS—Special considerations for application
    * ASK_AMT—Funding amount requested
    * IS_SUCCESSFUL—Was the money used effectively

- The target variable is STATUS
- The feature variables are:
    * APPLICATION_TYPE—Alphabet Soup application type
    * AFFILIATION—Affiliated sector of industry
    * CLASSIFICATION—Government organization classification
    * USE_CASE—Use case for funding
    * ORGANIZATION—Organization type
    * INCOME_AMT—Income classification
    * SPECIAL_CONSIDERATIONS—Special considerations for application
    * ASK_AMT—Funding amount requested
    * IS_SUCCESSFUL—Was the money used effectively
- The EIN and NAME—Identification columns were deleted because they didn't provide valuable data to our model.

#### 2. Compiling, Training, and Evaluating the Model
   - The model has 305 neurons, four layers, a reLu activation function on hidden layers, and sigmoid activation function on the output layer. Using the reLu function on hidden layers is a common practice because it is nonlinear yet fast and does not suffer from vanishing gradient problems, and the sigmoid function is a great function for returning probability. I used 128 neurons per hidden layer because it is more than multiple of the input layer's nods, and using a  number that is power of two is efficient for modern hardware.
     ![](https://github.com/MahsaBakhtiari/GrantworthyAI/blob/main/pics/1.png)
   - The model is performing almost perfect with the acuracy of 99.98% on the test data.
   - Choosing the right number of nurons, and suitable activation functins and efficient data preprossesing all end up emprove model performance.
     ![](https://github.com/MahsaBakhtiari/GrantworthyAI/blob/main/pics/2.png)


    
    
    
    
