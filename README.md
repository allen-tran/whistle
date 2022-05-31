# Whistle 🌬

A simple TCP chat room written in GoLang. This application allows clients to connect to port `8001`, create a username or be ✨anonymous✨, and start joining rooms to send a message.

![image](https://user-images.githubusercontent.com/63386979/171106532-eef32fbe-b96b-42e3-a0e0-79b38e0912e1.png)

## Demo 🎯

<img width="1143" alt=" 2022-05-30 at 11 59 30 PM" src="https://user-images.githubusercontent.com/63386979/171111861-19c9699f-cb9b-439a-89aa-8b54c36139aa.png">
Here is an example of two clients connected via TCP on Whistle. They were able to create nicknames and join a room to chat with each other. After they were doing, they quit out of the rooms.

## Usage 🚀
### 1. Clone the Repository
```
$ git clone https://github.com/allen-tran/whistle/
```
### 2. Run the App
```
$ ./whistle
```
### 3. Connect the Client

#### MacOS
`$ nc ::1 8001`
#### Linux
`$ telnet localhost 8001`

## Commands 🎮
- `/nick <name>`: give yourself a nickname, else stay anonymous
- `/join <name>`: join a room. if the room does not exist, it will be created for you
- `/rooms`: show list of availible rooms
- `/msg <message>`: broadcast message to everyone in room
- `/quit`: disconnects from chat server
