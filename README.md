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
