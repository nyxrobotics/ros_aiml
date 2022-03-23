# Chatbot-ros-package
### Setup
- Add execution permission
```
cd scripts
chmod +x ./*
cd ..
```
- Isntall AIML
```
pip install aiml
```
- Fix your workspace path in tts_chat.launch
```
<param name="aiml_path" value="/home/kronton/localbot_ws/src/ros_aiml/data" />
```
- launch tts_chat.launch
```
roslaunch ros_aiml tts_chat.launch

```
- If you use voice from "festival" (such as 'voice_us1_mbrola'), install it
```
sudo apt install ros-melodic-audio-common ros-melodic-sound-play
sudo install festvox-us1

```
- Check available voices [](https://codeantenna.com/a/9dIOaSVQVD)

```
ls /usr/share/festival/voices/english 
```

```
sudo apt-cache search --names-only festvox-* 
```
- Edit aiml_tts_client.py to change the voice
```
	soundhandle.say(response,'voice_us1_mbrola')
```
