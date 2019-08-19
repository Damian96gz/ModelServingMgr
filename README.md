# Overview
This is a tool to quickly save your machine learning models and deploy them on k8s or docker-compose for serving purpose.

<br/>

# Support

- Serve Tensorflow .pb models
- Serve Pytorch models
- Serve MXNet models
- Serve SKLearn models
- Serve other machine learning models saved in .onnx form 


<br/>

# Functions:
### 1:MLModelMgmt: 
Build an image, convert and save your trained models to this serviceable image

**apis：**
- MLModelMgmt.build_image
- MLModelMgmt.push_image
- MxnetToOnnx.build_image
- PytorhcToOnnx.build_image
- SklToOnxx.build_image

You can check the api documents for more information about these apis


<br/>

### 2:FeedMeImages: 
Use the model saving images and a serving image to serve your model on k8s or docker-compose

**apis:**

- MxnetServing.k8sYaml
- MxnetServing.composeYaml
- OnnxServing.k8sYaml
- OnnxServing.composeYaml
- TfServing.k8sYaml
- TfServing.composeYaml

You can check the api documents for more information about these apis

<br/>

# Pre-request:

- Python3.6+
- Docker-ce
- onnx
- tensorflow
- torch
- torchvision
- mxnet
- skl2onnx
- minikube or kubernetes(if you want to serve it on k8s)
- docker-compose(if you want to serve it with docker-compose)

<br/>

# Example:

<br/>

# Install the package:
```
git clone <url> 

cd feedmeimages-master

python setup.py install
```
