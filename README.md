# Deep Learning Methods for Lung Ultrasound Classification
An automated ultrasound screening system which takes in the ultrasound clips as input, converts them into frames and filters out relevant frames using frame selection techniques, trains a model on the frames and predicts the presence of pneumonia.

## Data
Store the videos in a folder directory named "Lung ultrasound exams_MovieClips/Lung ultrasound exams/{Patient_id}" according to the corresponding Patient_id

Store the model pickle files in a folder named "model_weights"

## Method
Two main parts of the method and their corresponding python notebook files:
1. Clips to frame conversion and frame selection:
This is the part wherein the Ultrasound Clips are first converted to frames using different methods such as Skip 0 frame, Skip 1 frame and Skip 2 frames. Once this conversion is done, we filter out the frames based on two selection methods namely Max Brightness selection and Middle 50% selection method. 
The notebook file corresponding to this is:
"Clips to frame conversion and frame selection.ipynb"
2. Modelling:
This is the part wherein the frames are loaded into the 2 types of model architectures used in this paper namely CNN + DenseNet and CNN + DenseNet + ML Classifier. 
The notebook file corresponding to this is:
"Modelling.ipynb"

Steps to run:
1. You need to run the "Clips to frame conversion and frame selection.ipynb" first to load all the videos and convert them into frame inputs. The process is well explained in the notebook and the code flow is one-directional. There are different code snippets to run from on the basis of the frame selection method you need.
2. Once the whole notebook is run, you will get the frames according to the frame selection method you used. Then you need to run the "Modelling.ipynb" notebook. The code flow here has been divided into different steps and this has been mentioned clearly in the Markdown cells. Two types of model architectures namely CNN + DenseNet and CNN + DenseNet + ML Classifier are run and the codes follow this order. Once you run the whole notebook, the final results will be displayed with the accuracy metrics.

## CNN + DenseNet-201 architecture:
![CNN_Architecture](https://github.com/user-attachments/assets/0469f010-d337-45cd-b50b-5e4ad9bc402a)

### Additional details about the dataset will be provided upon request
