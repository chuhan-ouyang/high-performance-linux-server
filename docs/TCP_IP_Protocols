## bottom data layer (kernel)
* drivers for network cards
* convert between IP address and physical address (eg. MAC)
* ARP/RARP

## networking layer (kernel)
* route and sending of packets
* choose nodes
* IP: choose routing/hopping based on the IP destination address of the packet

## transpot layer (kernel)
* end to end communication
* only care about start and end terminals
* logical connection between ends responsible for resending and reconnection of data
* TCP: reliable, stream service
  * reconnection, acks to make sure data gets send
  * must establish TCP connection first
  * store (in kernel) data structures about connection status/ rw buffers
  * release data in kernel when connection finishes
  stream
* UDP
  * unreliable, no connection 
  * can't promise data gets send from end to end
  * if data gets lost, user app need to implement reconnection itself
  * no stream: fixed length
* SCTP

## applciation layer (user)
* file transmission, network management
* ping

## encapsulation
* upper layer cascade down
* include header info
* when terminal use 'send" to write data into TCP connection, kernel copies data into buffer, TCP invokes IP (pass in header info and buffer)
* udp datagram
* ip datagram
* encpsulated in bottom data layer -. frame

## usage
* bubble up
* use header info to distinguish between higher layer protocol

## ARP
* 
