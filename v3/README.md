## WWN Boundary Interfaces and Components

<img src="https://raw.githubusercontent.com/waggle-sensor/wild-waggle-node/main/v3/images/WSN.png" width="900"></br>


| Port | Description | Use/Notes |
| ------------- |------------- | ------------- |
|**AC Power**|3 pin single phase 50/60 Hz, 85-264 VAC power input. | AC power input for the nodes.| 
|**Power LED**|Red LED that indicates power to the Node.|The LED turns on about 16 seconds after applying power.|
|**Status LED**|Multicolored LED that shows the status of the Node. | _Blinking blue_: the WSN is booted and running. _Solid red_: the WSN is shut down, and power can safely be removed.|
|**Health LED**|Multicolored LED that shows the health node.|_Solid green_: Healthy state. _Solid Orange_: Warning state -- one or more minor issues. _Solid Red_: Failed state-- one or more major issues. LED should transition from off to solid green about 10 min after power ON. If the LED is not green, check back after approximately 1 hour.|
|**WAN**|Gigabit Ethernet RJ-45 port.| Default network interface for the node. Its use may be needed for initial provisioning and post-install debugging.|
|**Sen 1-4 (POE)**|Interface port with POE capability. 30W max power, DHCP addressing. Sensors connected here are accessible by all processing modules in the node.| Cameras and Stevenson shield that are part of the standard node use these ports. One or more ports may be available for interfacing additional sensors.|
|**Sen 5**|Interface port with USB2 support. Sensor connected to this port is available only to the 1st processing module in the node.| Generally available to interface a legacy USB sensor. The POE is the recommended interface to add new sensors to the instrument. Compatible cable can be obtained [here.](https://www.usbfirewire.com/parts/rr-111220-06-xx.html#RR-111220-06-39)|
|**Air Vent**|Gore-tex vent for venting moisture safely.| This vent should not be covered. It keeps the main processor box free of moisture and condensation.|
|**Console**|Debugging serial console.| Easy-access serial console used for debugging by the devOps team.|
