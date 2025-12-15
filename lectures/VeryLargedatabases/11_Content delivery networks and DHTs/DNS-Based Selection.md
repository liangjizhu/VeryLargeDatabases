A technique where [[Domain Name System (DNS)]] responses are used to choose which server or replica a client should contact.
Many [[Domain Name System (DNS)]] implementations allow the Web site [[Domain Name System (DNS)]] to map a host domain name to a set of IP addresses and choose on of them for every query
Advantages:
- Avoid [[TCP or IP]] set-up delay
- [[Domain Name System (DNS)]] reduces overhead
- Relatively fine control
Disadvantages:
- "Hidden load" effect
- [[Domain Name System (DNS)]] [[Time To Live (TTL)]] limits adaptation
- Based on the IP address of the local [[Domain Name System (DNS)]] server