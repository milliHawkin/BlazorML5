# ML5 For Blazor
 
 ### My attempt to use ML5 library from Blazor WASM

#### Features
1. Neural Network 
2. Image Classification

#### Demo
1. [Color Classifier](https://github.com/sps014/Color-Classifier-Demo-Source) Training in Browser With Neural Network


#### Usage


 ##### Image Classifier
 
 1. Creating Classifier
  ```C#
 ImageClassifier classifier = new ImageClassifier(jsruntime, ImageModel.MobileNet);//BuiltIn Model
 ImageClassifier classifier = new ImageClassifier(JSRuntime, "path/to/wwwroot/model/or/url"); //Custom Teachable Machine
  ```
 2. events
 ```C#
  classifier.OnModelLoad+=ModelLoaded;
         
 /// when Model Loaded
 void ModelLoaded()
 {
      //do prediction
 }
