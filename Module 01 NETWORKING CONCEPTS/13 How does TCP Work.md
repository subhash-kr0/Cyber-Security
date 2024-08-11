# How Does TCP Work?

## English Version

**TCP (Transmission Control Protocol)** is one of the core protocols of the Internet Protocol Suite. It is responsible for ensuring reliable, ordered, and error-checked delivery of data between applications running on devices connected to a network.

### Key Features of TCP

1. **Connection-Oriented:**
   - TCP establishes a connection between the sender and receiver before data transmission begins. This connection setup involves a process known as the **three-way handshake**.

2. **Three-Way Handshake:**
   - **Step 1: SYN:** The sender sends a synchronization (SYN) packet to the receiver to initiate the connection.
   - **Step 2: SYN-ACK:** The receiver responds with a synchronization-acknowledgment (SYN-ACK) packet, acknowledging the receipt of the SYN packet.
   - **Step 3: ACK:** The sender sends an acknowledgment (ACK) packet back to the receiver, confirming the establishment of the connection.

3. **Data Segmentation:**
   - Large data messages are divided into smaller segments. Each segment is assigned a sequence number to ensure the data can be reassembled in the correct order at the destination.

4. **Error Detection and Correction:**
   - TCP uses checksums to detect errors in the transmitted data. If an error is detected, TCP requests the retransmission of the affected segment.

5. **Flow Control:**
   - TCP uses a flow control mechanism to ensure that the sender does not overwhelm the receiver with too much data at once. This is achieved through the use of a sliding window protocol, which controls the amount of data that can be sent before receiving an acknowledgment.

6. **Congestion Control:**
   - TCP monitors network traffic to adjust the rate of data transmission, preventing network congestion. It uses algorithms like **Slow Start**, **Congestion Avoidance**, **Fast Retransmit**, and **Fast Recovery** to manage congestion.

7. **Connection Termination:**
   - When data transmission is complete, TCP performs a graceful termination of the connection using a four-way handshake process to ensure both sides have finished the data exchange.

### How TCP Works

1. **Connection Establishment:**
   - TCP begins with the three-way handshake to establish a connection. This process ensures that both the sender and receiver are ready for data transmission.

2. **Data Transfer:**
   - Data is sent in segments, each with a sequence number. The receiver sends acknowledgments for successfully received segments. If a segment is lost or corrupted, TCP requests retransmission.

3. **Data Reassembly:**
   - At the receiver’s end, TCP reassembles the data segments based on their sequence numbers to reconstruct the original message.

4. **Connection Termination:**
   - Once data transfer is complete, TCP terminates the connection using the four-way handshake, ensuring that all data has been transmitted and acknowledged.

## Hinglish Version

**TCP (Transmission Control Protocol)** Internet Protocol Suite ke core protocols me se ek hai. Yeh responsible hota hai reliable, ordered, aur error-checked delivery of data ko ensure karne ke liye applications ke beech jo devices network pe connected hain.

### TCP ke Key Features

1. **Connection-Oriented:**
   - TCP sender aur receiver ke beech ek connection establish karta hai data transmission shuru hone se pehle. Yeh connection setup ek process ke through hota hai jo **three-way handshake** kehlata hai.

2. **Three-Way Handshake:**
   - **Step 1: SYN:** Sender ek synchronization (SYN) packet receiver ko bhejta hai connection initiate karne ke liye.
   - **Step 2: SYN-ACK:** Receiver synchronization-acknowledgment (SYN-ACK) packet ke saath response karta hai, SYN packet ke receipt ko acknowledge karta hai.
   - **Step 3: ACK:** Sender ek acknowledgment (ACK) packet receiver ko bhejta hai, connection establish hone ki confirmation ke liye.

3. **Data Segmentation:**
   - Badi data messages ko chote segments me divide kiya jata hai. Har segment ko sequence number assign kiya jata hai taaki data destination par sahi order me reassemble ho sake.

4. **Error Detection aur Correction:**
   - TCP checksums use karta hai transmitted data me errors detect karne ke liye. Agar error detect hota hai, TCP affected segment ke retransmission ko request karta hai.

5. **Flow Control:**
   - TCP ek flow control mechanism use karta hai taaki sender receiver ko ek baar me zyada data na bheje. Yeh sliding window protocol ke through achieve kiya jata hai, jo data send karne se pehle acknowledgment receive karne tak ka amount control karta hai.

6. **Congestion Control:**
   - TCP network traffic monitor karta hai taaki data transmission rate adjust kar sake, network congestion prevent karne ke liye. Yeh algorithms jaise **Slow Start**, **Congestion Avoidance**, **Fast Retransmit**, aur **Fast Recovery** use karta hai congestion manage karne ke liye.

7. **Connection Termination:**
   - Data transmission complete hone ke baad, TCP ek graceful termination perform karta hai connection ka using four-way handshake process taaki dono sides data exchange finish hone ki confirmation de sake.

### TCP Kaise Kaam Karta Hai

1. **Connection Establishment:**
   - TCP three-way handshake se connection establish karta hai. Yeh process ensure karta hai ki sender aur receiver data transmission ke liye ready hain.

2. **Data Transfer:**
   - Data segments me bheja jata hai, har segment ke saath sequence number hota hai. Receiver successfully received segments ke liye acknowledgments bhejta hai. Agar segment lost ya corrupted hota hai, TCP retransmission request karta hai.

3. **Data Reassembly:**
   - Receiver ke end pe, TCP data segments ko unke sequence numbers ke basis pe reassemble karta hai original message reconstruct karne ke liye.

4. **Connection Termination:**
   - Data transfer complete hone ke baad, TCP connection ko four-way handshake ke through terminate karta hai, ensure karta hai ki saara data transmit aur acknowledge ho chuka hai.
