## OSI MODEL
---
OSI- Open System Interconnection. 
- A & layer arch. with each layer having specific functionality to perform.
- All these 7 layers work collaboratively to transmit the data from one person to another across the globe.

![[OSI.png]]

---
### **1. #Physical-Layer (Layer 1) :**
- The lowest layer of the OSI reference model is the physical layer. 
- It is responsible for the actual physical connection between the devices. 
- The physical layer contains information in the form of **bits.**
- It is responsible for transmitting individual bits from one node to the next. 
- When receiving data, this layer will get the signal received and convert it into 0s and 1s and send them to the Data Link layer, which will put the frame back together.

![[physical.png]]

#### Functions of Physical Layer

1.  **Bit synchronization:** The physical layer provides the synchronization of the bits by providing a clock. This clock controls both sender and receiver thus providing synchronization at bit level.
2.  **Bit rate control:** The Physical layer also defines the transmission rate i.e. the number of bits sent per second.
3. 	3.  **Physical topologies:** Physical layer specifies the way in which the different, devices/nodes are arranged in a network i.e. bus, star, or mesh topology.
4.  **Transmission mode:** Physical layer also defines the way in which the data flows between the two connected devices. The various transmission modes possible are Simplex, half-duplex and full-duplex.
---
