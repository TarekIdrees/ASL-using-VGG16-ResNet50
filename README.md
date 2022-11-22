# ASL-using-VGG16-ResNet50
> Two different architecture of CNN (VGG16 - ResNet50 ) to predict the sign language of ASL images with accuracy 99%

> ASL is a complete and organized visual language that is expressed by facial expression as well as movements and motions with the hands.

> CNN models build on GRY data.
 
# Architecture:
> VGG16 model
- Built in VGG16 model.

- Flatten

- Dense : [420, activation = relu]
- Dense : [29, activation = softmax]

> ResNet50 model

- Built in ResNet50 model

- Flatten

- Dense : [420, activation = relu]
- Dense : [29, activation = softmax]

# Accuracy 
> VGG16 model accuracy on training data : 99.8%

> ResNet50 model accuracy on training data : 99.6%

# Data augmentation
> augment the data with ImageDataGenerator to avoid overfiting.

# Data
>The data set is a collection of images of alphabets from the American Sign Language, separated in 29 folders which represent the various classes.

> The ASL Alphabet data set provides 87,000 images of the ASL alphabet.

> The test data set contains a mere 29 images, to encourage the use of real-world test images.

> There are 2 data sets utilized in this notebook:
 - *ASL Alphabet train* - This data set is the basis for the model.
 - *ASL Alphabet Test* - This data set was made specifically for validating the model created using the above data set, and is intended to be used to improve the feature engineering and modeling process to make it more versatile in "the wild" with less contrived images.

> It is available on Kaggle as the ASL Alphabet Dataset. https://www.kaggle.com/grassknoted/asl-alphabet.

# Functions 
> *load_train_data*
```
function to load train data in GRAY type.
```
> *load_test_data*
```
function to load test data in GRAY type.
```
## Credits [EngMohamadIdrees](https://github.com/EngMohamadIdrees) -[Tarek Idrees](https://github.com/TarekIdrees) - [Mohamed Mahmoud](https://github.com/Thesnak)
