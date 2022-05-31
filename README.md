# Whistle

A simple TCP chat room written in GoLang. This application allows clients to connect to port `8001`, create a username or be ✨anonymous✨, and start joining rooms to send a message.

![image](https://user-images.githubusercontent.com/63386979/171106532-eef32fbe-b96b-42e3-a0e0-79b38e0912e1.png)

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
```
$ nc ::1 8001
```
#### Linux
```
$ telnet localhost 8001
```
#### Windows

not sure, please see [netstat](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/netstat)

## Commands 🎮
- `/nick <name>`: give yourself a nickname, else stay anonymous
- `/join <name>`: join a room. if the room does not exist, it will bhe creted for you.
- `/rooms`: show list of availible rooms
- `/msg <message>`: broadcast message to everyone in room
- `/quit`: disconnects from chat server
