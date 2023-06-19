# tchrs-opencv-webcam-inference 
This example shows steps for running a Python trained model on webcam feed with opencv and tch-rs. Model will run on GPU.

Model used in example is mobilenet_v3_small. It is trained on Cifar10 dataset for 10 epochs. Python training and testing scripts are included in: 
```
/train_simple_classifier
```
Add the following dependencies:
```
cargo add tch anyhow opencv
```
main.rs is commented for readers to understand easily.

Pretrained model and a test video also included in repo

# Usage
To run example on a video use below command:
```
cargo run cifar10_mobilenet_v3_small.pt test_video.mp4
```
To run example on your webcam use below command:
```
cargo run cifar10_mobilenet_v3_small.pt /dev/video0
```
