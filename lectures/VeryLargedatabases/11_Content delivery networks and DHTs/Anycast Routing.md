A network addressing and routing technique where multiple servers share the same IP address, and the network routes a client’s request to the “closest” or best server according to routing metrics.
- Multiple physical servers use a single IP address called anycast address
- Each server advertises both the anycast address and its regular address
- Routers build paths that lead to the nearest anycast member-server
Advantages:
- No extra [[Round-Trip Time (RTT)]]
- Route to a nearby server
Disadvantages
- Does not consider network or server load
- Different packets may go to different servers
- Used only for simple request-response apps