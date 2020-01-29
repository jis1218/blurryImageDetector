##### data augmentation

https://www.pyimagesearch.com/2019/07/08/keras-imagedatagenerator-and-data-augmentation/

##### data augumentation을 하니 확실히 학습이 잘 된다.
```python
train_image_generator = ImageDataGenerator(rescale=1./255, #밑에 추가됨
                                          rotation_range=45,
                                          width_shift_range=.15,
                                          height_shift_range=.15,
                                          horizontal_flip=True,
                                          zoom_range=0.5) 
validation_image_generator = ImageDataGenerator(rescale=1./255, #밑에 추가됨
                                               rotation_range=45,
                                              width_shift_range=.15,
                                              height_shift_range=.15,
                                              horizontal_flip=True,
                                              zoom_range=0.5)
```