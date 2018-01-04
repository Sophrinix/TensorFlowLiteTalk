# TensorFlowLiteTalk
On January 18 2018 this is the repo for a talk on TensorFlow Lite + CoreML for iOS. 

In this talk we will we will discuss what TensorFlow Lite is, why it is needed, and what you can do with on iOS and Android. I'll largely ignore Raspberry Pi. 

On the iOS side we will discuss CoreML and how we can convert a TensorFlow Lite and even a Keras Model to CoreML and take advantage of the GPU on iOS.

The follow along labs will use Docker for the Android Examples.

## Getting Docker
#### Please have Docker installed before the talk
 [Docker for Windows 10](https://store.docker.com/editions/community/docker-ce-desktop-window)
[Docker for MacOS](https://store.docker.com/editions/community/docker-ce-desktop-mac)
Docker for Linux (Ubuntu) 
 ```sudo apt-get install docker```

 [Source for the open bits of Docker. (You don't need this, this just for information purposes)](https://github.com/moby/moby)

 ## Slides (Reveal JS)
 launching the sides locally:
 ```cd slides\ && grunt ```
 Then open a browser and go to ```http://localhost:3000```

To Follow along with my slides (websocket broadcast):
In a browser go to ```http://<My_IP_Address>:3000/client```
My_IP_Address will be determined at the time of the talk.

 ### Jupyter Notebook (From Docker)
 ``` cd labs/tensorflow-jupyter```

 ```docker run -it --rm -p 8888:8888 jupyter/tensorflow-notebook```

 ### Chat Lab (From Docker)
 ``` cd labs/chatbot```

 ```docker run -it --rm -p 8888:8888 chatbot```

### Image Classifier (From Docker)
 ``` cd labs/image-classifier```

 ```docker run -it --rm -p 8888:8888 image-classify-android```

 ### Face Recognition (Cross Platform) (From Docker)
 ``` cd labs/face-recognition-cross-platform```

 ```docker run -it --rm -p 8888:8888 facerecognition```

 ### CoreML Lab
  ```docker run -it --rm -p 8888:8888 coreml-converter```
  You will need a mac to run the converted model.
  If you do have Mac then also run ```open digitrecognize.xcproj```

