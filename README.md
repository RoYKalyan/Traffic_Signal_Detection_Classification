# Traffic Sign Recognition for Autonomous Vehicles

## Abstract

Deep learning and automotive advancements are driving the development of smart cars and autonomous vehicles. Traffic sign recognition, essential for safe autonomous driving, is being tackled with innovative deep-learning techniques. These signs are paramount for global traffic flow and driver safety. Recognizing them improves driver assistance systems and the driving experience in general. While challenges like weather variations and sign degradation exist, Smart Driving Support Systems offer promising solutions for both Advanced Driver-Assistance Systems and future autonomous vehicles.

Our research introduces two novel CNN architectures, namely the TS-Net and TSDetector CNN models, trained on the 'German Traffic Sign Detection Benchmark' (GTSDB) dataset. The goal is to improve traffic sign detection and classification accuracy and contribute to the progression of autonomous vehicle technology, ultimately mitigating traffic accidents.

In the object detection task, our custom TSDetector model outperformed both FasterRCNN and RetinaNet. For classification, the pre-trained ResNet50 model achieved the highest accuracy, surpassing MobileNetV2 and the custom TS-Net. Our aspiration is for these models to surpass traditional methods, thereby further unlocking the potential of custom deep-learning architectures for real-world autonomous driving applications.

## Keywords

Deep Learning, Traffic Sign Recognition, Autonomous Vehicles, CNN, GTSDB.


# Data Collection

The experimentation utilized the German Traffic Sign Detection Benchmark (GTSDB), introduced at the IEEE International Joint Conference on Neural Networks 2013. The dataset is publicly available [here](https://benchmark.ini.rub.de/gtsdb_dataset.html). It comprises 900 images containing 1206 traffic signs, divided into a training set of 600 images and a testing set of 300 images, stored in Portable Pixmap (ppm) format. The signs vary in size from 16x16 to 128x128 pixels and may appear singly or in multiples, with variations in orientation, lighting, and occlusions.

The signs are categorized into four types: mandatory, prohibitory, danger, and other. However, signs labeled as "other" are irrelevant to the challenge and thus excluded. The training set contains 396 prohibitory (59.5%), 114 mandatory (17.1%), and 156 danger (23.4%) sign samples, while the testing set comprises 161 prohibitory, 49 mandatory, and 63 danger sign images.

The dataset encompasses 43 different traffic sign classes, commonly found worldwide. Dataset statistics are depicted below:

### Statistics of Our GTSDB Dataset

| Data Split | Training | Test | Total |
|------------|----------|------|-------|
| Numbers    | 600      | 300  | 900   |

### Traffic Sign Classification Labels

#### Part 1

| ID | Description                | Type        |
|----|----------------------------|-------------|
| 0  | speed limit 20             | prohibitory |
| 1  | speed limit 30             | prohibitory |
| 2  | speed limit 50             | prohibitory |
| 3  | speed limit 60             | prohibitory |
| 4  | speed limit 70             | prohibitory |
| 5  | speed limit 80             | prohibitory |
| 6  | restriction ends 80        | other       |
| 7  | speed limit 100            | prohibitory |
| 8  | speed limit 120            | prohibitory |
| 9  | no overtaking              | prohibitory |
| ...| ...                        | ...         |

#### Part 2

| ID | Description                | Type        |
|----|----------------------------|-------------|
| 21 | bend                       | danger      |
| 22 | uneven road                | danger      |
| 23 | slippery road              | danger      |
| 24 | road narrows               | danger      |
| ...| ...                        | ...         |

### Traffic sign images of all the 43 classes:

![Traffic sign images](https://www.researchgate.net/publication/367980634/figure/fig4/AS:11431281117125287@1675382530134/Forty-three-kinds-of-German-traffic-signs-from-GTSDB-dataset.ppm)


