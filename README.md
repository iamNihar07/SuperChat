# CSE-3310-SuperChat Group 7 <br />
Team members: Alex Eseyin, David Miller, Henry Le, Nihar Gupte <br />

Superchat created for CSE 3310 - Spring 2019 <br />

Uses basic ASIO networking protocol and ncurses for GUI <br />
<br />
to compile: <br />
make <br />
<br />
to run: <br />
./chat_server 9000 in one command window <br />
./chat_client 127.0.0.1 9000 in separate command window <br />
<br />
Help menu for superchat: <br />
the avaliable commands: <br />
        /c <room name> creates a room called <room name> <br />
        /e <room name> enters a room called <room name> <br />
        /d <room name> deletes a room called <room name> <br />
        /b <user name> blocks the user called <user name> <br />
        /u <user name> unblocks the user called <user name> <br />
        /h displays this help menu <br />
        /q exits the program <br />
        to enter lobby type /e Lobby <br />
        Chatrooms can only be deleted if there are no active users in it <br />
<br />
        
# How to Run
The following commands should be run in the terminal before the program is run.
     
    sudo apt-get install libboost-all-dev
    sudo apt-get install libncurses5-dev

     
After Installing the above packages, type the command below to make the executables.

    make
    
The client and server can be run on different terminals or computers using the following commands

    ./chat_server <port_number>
    ./chat_client <IP_Address > <port_number>
  
# Note
The port number should be the same for the clients and the server to send and recieve messages between different clients.

# Commands Supported
The follwing commands are supported in the application:

1.   /help

          This Command lists all the commands supported on the terminal.
2.   /quit
          
          Quits the program.
3.   /change chatroom
          
          This command lists all the available chatrooms and allows the user to create chatrooms and change between them.
4.   /delete chatroom

          This command lets the user delete a chatroom. A chatroom cannot be deleted if there is a client inside it. The Main lobby cannot be deleted.
5.   /ban

          Bans the client specified. All messages from the banned users are ignored.
6.   /unban

          Allows the user to unban the banned users.
