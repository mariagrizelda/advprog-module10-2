# Tutorial 10 - Broadcast Chat
**Maria Helga Grizelda - 2206046733**

## 2.1 Original Code & How It Runs
<img src="image/Screenshot 2024-05-08 at 18.48.51.png">
Upon executing the server with cargo run --bin server and launching each client using cargo run --bin client, the output demonstrates that all clients and the server receive chat messages broadcasted by every other client. When a client inputs a message in the command line, it gets transmitted to the server, which then relays it to all connected clients. This mechanism ensures that each participant in the network can observe messages from all other clients, fostering a real-time, multi-user chat environment.

## 2.2 Modifying the websocket port
<img src="image/Screenshot 2024-05-08 at 18.58.29.png">

To ensure functionality, it's essential to synchronize the ports specified in both client.rs and server.rs. If these files designate different ports, the client won't be able to establish a connection with the server. Aligning the ports is critical to ensure a successful connection between the client and the server.

## 2.3 Small Changes
<img src="image/Screenshot 2024-05-08 at 19.05.43.png">

At this stage, we incorporate sender information for each client, comprising both the IP and Port. This addition enables clients to discern the source of each message. When bcast.tx (the sender) disseminates messages to its subscribers, it includes the sender's IP extracted from the text via the addr variable. This enhancement enriches communication by offering clear sender identification alongside every message.




