# Keras webapp for Image Classifier


```shell
$ cd keras_webapp
$ docker build -t keras_webapp .
```

### Build and run an image for keras-application pretrained model 
```shell
$ docker run -d -p 55000:5000 keras_webapp
```
# OR

### Build and run the image from your model into the container.
```shell
$ docker run -e MODEL_PATH=/mnt/models/your_model.h5  -v volume-name:/mnt/models -p 55000:5000 keras_webapp
```
now go to 
http://localhost:55000
