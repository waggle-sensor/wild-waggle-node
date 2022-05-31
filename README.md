# Wild Waggle Node (WWN)

Following a modular design, nodes enable rapid integration of new sensor technologies, from LIDAR to precision micro-synchrophasors for analysis of electrical distribution systems. Wild Waggle Nodes are weatherized for remote, outdoor deployment in remote and hard-to-reach locations. An important feature of our design is the addition of resilience software and hardware elements. The Waggle manager, [Wagman](https://github.com/waggle-sensor/wagman), is a custom circuit board for environment and health monitoring, and actively controlling power. Wagman can disconnect malfunctioning devices or reboot components with backup software stacks, providing robust operation in remote and harsh locales. The next most important device in a WWN is the [Node Controller](https://github.com/waggle-sensor/nodecontroller). It is a single-board Linux computer providing encrypted TCP/IP messaging, data caching, node health monitoring, and cybersecurity tools including cryptokey management and signed software. While the above tasks are its main priority, through container-based isolation technologies, the node controller is also available to run [user applications](https://github.com/waggle-sensor) on the dedicated CPU-GPU resources. Additional processing and storage elements can now be added to this basic construct, and they are called [Edge Processors](https://github.com/waggle-sensor/edge_processor). A collection of components that provide power, networking, and embedded interfacing capabilities complete the basic node. This node can now be extended with sensors through standard Ethernet ([POE](https://en.wikipedia.org/wiki/Power_over_Ethernet)), USB and other [embedded protocols](https://en.wikipedia.org/wiki/Communication_protocol).
