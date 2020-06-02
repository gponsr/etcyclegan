#ET-CycleGAN: Emotion-guided Thermal CycleGAN

This code is based on the work of Jun-Yan Zhu et al. https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix/
Copyright (c) 2017, Jun-Yan Zhu and Taesung Park
All rights reserved.


## Training the model

Download the pre-trained weights "ResNet50_EMO.pth" and "VGG19_FACE_checkpoint.pth.tar" and copy them in "./models/checkpoints/"

```
python train.py --dataroot path_to_data --name name_experiment --model cycle_gan --phase train
```

## Testing the model

Rename first: "./checkpoints/name_experiment/latest_net_G_A.pth" to "./checkpoints/name_experiment/latest_net_G.pth"

```
python test.py --dataroot path_to_data/testA --name name_experiment --model test --no_dropout
```



