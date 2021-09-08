<h1 align="center">CAM-DUMPER</h1>
<p align="center"><img src="cd.jpg" max-width="90%%" height="auto"></p>
<p align="center">Take webcam shots from target by just sending a malicious link</p>

# How it works?
<p>The tool generates a malicious HTTPS page using Serveo or Ngrok Port Forwarding methods, and a javascript code to cam requests using MediaDevices.getUserMedia. </p>

<p>The MediaDevices.getUserMedia() method prompts the user for permission to use a media input which produces a MediaStream with tracks containing the requested types of media. That stream can include, for example, a video track (produced by either a hardware or virtual video source such as a camera, video recording device, screen sharing service, and so forth), an audio track (similarly, produced by a physical or virtual audio source like a microphone, A/D converter, or the like), and possibly other track types. </p>

[See more about MediaDEvices.getUserMedia() here](https://developer.mozilla.org/en-US/docs/Web/API/MediaDevices/getUserMedia)

## Installing (Kali Linux/Termux):

```
$ apt update && apt upgrade
```
```
$ apt install git
```
```
$ apt install php wget curl jq
```
```
$ git clone https://github.com/LiNuX-Mallu/CAM-DUMPER.git
```
```
$ cd CAM-DUMPER
```
```
$ wget https://bin.equinox.io/c/4VmDzA7iaHb/ngrok-stable-linux-arm.zip && unzip *.zip && rm *.zip
```
```
$ chmod +x camdumper.sh ngrok
```
```
$ echo "web_addr: 4045" >> $HOME/.ngrok2/ngrok.yml
```
```
$ ./camdumper.sh

```
if $HOME/.ngrok2/ngrok.yml doesnt exist then
you must create it by running-
```
$ mkdir $HOME/.ngrok2 && touch $HOME/.ngrok2/ngrok.yml
```
