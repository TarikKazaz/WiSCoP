# WiSCoP - Wireless Sensor Communication Prototyping Platform

## Abstract
To enhance system performance of future heterogeneous wireless networks the co-design of PHY, MAC, and higher
layer protocols is inevitable. In this work, we present WiSCoP- a novel embedded platform for experimentation, prototyping
and implementation of integrated cross-layer network design approaches. WiSCoP is an SDR-based implementation of the IEEE 802.15.4 (Zigbee)
standard built on top of a Zynq hardware platform integrated with FMCOMMS1/2/4 RF front-ends.
We demonstrate the flexibility of WiSCoP by using it to prototype a fully standard compliant IEEE 802.15.4 stack with real-time performance and cross-layer integration.
## Motivation

Traditional wireless industry solutions follow a layered design approach because it allows development of simple, modular and interoperable protocols. However, this principle causes information hiding between protocol layers, i.e. information about operation at one layer cannot be used by higher or lower layers. Therefore, radio chipset vendors offer limited coordination between physical
(PHY), medium access control (MAC), and higher-layer protocols. As a result, PHY and MAC layer innovations are usually prototyped separately without the possibility for joint optimization and real-world evaluation.

Novel PHY algorithms are typically prototyped on SDR platforms. These platforms consist of a RF front-end and a
host PC with CPU as main processing unit. However, CPUs cannot guarantee predictable processing latency due to its sequential
processing nature. This is the main reason why development of MAC algorithms that control SDR-based PHY
layer is extremely difficult. Moreover, such platforms have a large form factor and consume significant power which precludes
their distributed deployment. For these reasons, most MAC algorithms are developed and evaluated on embedded
platforms. Due to diverse radio chipset capabilities and hardware specifics, evaluating the same MAC layer algorithm on
different embedded platforms requires significant development time and effort. Furthermore, benchmarking innovative
cross-layer PHY/MAC optimized algorithms on diverse platforms is almost impossible.

To tackle this challenge, we present WiSCoP, a novel platform for prototyping cross-layer optimized protocols for WSNs.

## WiSCoP

![wiscop](https://cloud.githubusercontent.com/assets/4747573/26790552/757f5f46-4a14-11e7-9a63-83456affd48a.PNG)



WiSCoP is a FPGA-based real-time flexible IEEE 802.15.4 (Zigbee) PHY layer implemented in HDL on top of Xilinx Zynq SoC with additional
FMCOMMS1/2/4 RF front-ends, and drivers for flexible control of the IEEE 802.15.4 PHY layer  implemented in C.
The WiSCoP platform is shipped in form of a FPGA bitstream (executable) together with the aforementioned drivers in C, that provide
all the necessary interfaces for flexible radio/network control.
For more details see our publication.
To cite our work please use:

```
@article{kazaz2016demo,
  title={Demo: WiSCoP-Wireless Sensor Communication Prototyping Platform},
  author={Kazaz, Tarik and Jiao, Xianjun and Kulin, Merima and Moerman, Ingrid},
  journal={arXiv preprint arXiv:1612.02900},
  year={2016}
}
```


## Code
At this moment, the code for WiSCoP is available only on the internal Ghent University repositories, as decided by Ghent University.

## Contact
For more details do not hesitate to contact me:
**tarik.kazaz@ugent.be** or **tarik.kazaz@gmail.com**

## Ackowledgements
This work has been partially supported by the European Horizon 2020 Programs WiSHFUL and ORCA:

https://www.orca-project.eu/

http://www.wishful-project.eu/
