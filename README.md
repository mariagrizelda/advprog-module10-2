# Tutorial 10 - Broadcast Chat
**Maria Helga Grizelda - 2206046733**

## 2.1 Original Code & How It Runs
<img src="image/Screenshot 2024-05-08 at 18.48.51.png">
Upon executing the server with cargo run --bin server and launching each client using cargo run --bin client, the output demonstrates that all clients and the server receive chat messages broadcasted by every other client. When a client inputs a message in the command line, it gets transmitted to the server, which then relays it to all connected clients. This mechanism ensures that each participant in the network can observe messages from all other clients, fostering a real-time, multi-user chat environment.






