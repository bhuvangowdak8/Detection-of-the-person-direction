### DETECTING THE DIRECTION OF A PERSON
This application helps us in finding the direction in which the person is traversing. It is built on Nvidia Deepstream 5.1.

[Detection of person direction](https://github.com/user-attachments/assets/6aba5b6c-d1e2-40aa-bc1c-4efb83df9fb9)


## Deepstream Setup

This post assumes you have a fully functional Jetson device. If not, you can refer the documentation [here](https://docs.nvidia.com/jetson/jetpack/install-jetpack/index.html).

##  1. Install System Dependencies
```bash
sudo apt install \
libssl1.0.0 \
libgstreamer1.0-0 \
gstreamer1.0-tools \
gstreamer1.0-plugins-good \
gstreamer1.0-plugins-bad \
gstreamer1.0-plugins-ugly \
gstreamer1.0-libav \
libgstrtspserver-1.0-0 \
libjansson4=2.11-1
```
## 2. Install Deepstream
Download the DeepStream 5.1 Jetson Debian package deepstream-5.1_5.1.0-1_arm64.deb, to the Jetson device from [here](https://developer.nvidia.com/deepstream-getting-started). Then enter the command:

```bash
sudo apt install deepstream-5.1_5.1.0-1_arm64.deb
```
For more information, click [here](https://docs.nvidia.com/metropolis/deepstream/dev-guide/index.html).

## 3. Clone the repository
```bash
git@github.com:bhuvangowdak8/Detection-of-the-person-direction.git
cd person_direction_deepstream
```

## 4. Run the application

   I. To build the application
```bash
make
```
II. Now, run the application by providing the video source path 
```bash
./person_direction_deepstream <h264_elementary_stream>
```

## Please find the Link of a Demo video below
[Detection of person direction](https://www.youtube.com/watch?v=7tvSDLEeLqc)
