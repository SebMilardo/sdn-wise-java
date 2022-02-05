# sdn-wise-java
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/4681aa0b027a4eb79f935a08ba9bd01b)](https://www.codacy.com/gh/sdnwiselab/sdn-wise-java/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=sdnwiselab/sdn-wise-java&amp;utm_campaign=Badge_Grade)

The stateful Software Defined Networking solution for the Internet of Things. This repository contains a Java implementation of SDN-WISE. The repository is splitted into three folders:

* core: which contains the definitions of the flowtable, the packets, and some utility classes.
* ctrl: containing a small Java control plane that can be used to manage an emulated SDN-WISE network.
* data: an emulated SDN-WISE sensor node written in Java.

### Installation

Install Java, Maven and [RXTX](http://rxtx.qbang.org/wiki/index.php/Installation). On Ubuntu: 

```
sudo apt-get install openjdk-8-jdk maven librxtx-java  
```

Clone the GitHub repository and use Maven to build `sdn-wise-java`:

```shell
git clone https://github.com/sdnwiselab/sdn-wise-java.git
cd sdn-wise-java
mvn clean install
cd ctrl/build
java -jar sdn-wise-ctrl-X.X.X-jar-with-dependencies.jar 
```

When the network discovery is complete the SDN-WISE Java Control Plane GUI will popup. 
This GUI allows you to send a packet to a node, set/read the properties of a node, and check the content of its flowtable.


### Documentation 

[http://sdn-wise.dieei.unict.it](http://sdn-wise.dieei.unict.it/#Documentation)

### Versioning

* This project uses [semantic versioning](http://semver.org).

### Licensing

* See [LICENSE](LICENSE).

## Papers

Our approach is detailed in four scientific contributions:
```
@article{Anadiotis:2019,
  author    = {{Angelos-Christos} Anadiotis and Laura Galluccio and Sebastiano Milardo and Giacomo Morabito and Sergio Palazzo},
  title     = {{SD-WISE: A Software-Defined WIreless SEnsor network}},
  journal   = {Computer Networks},
  volume    = {159},
  pages     = {84 - 95},
  year      = {2019},
  doi       = {10.1016/j.comnet.2019.04.029},
  url       = {http://www.sciencedirect.com/science/article/pii/S1389128618312192},
}
```

```
@inproceedings{DiDio:2016,
  author    = {Paolo {Di Dio} and Salvatore Faraci and Laura Galluccio and Sebastiano Milardo and Giacomo Morabito and Sergio Palazzo and Patrizia Livreri},
  booktitle = {2016 Mediterranean Ad Hoc Networking Workshop (Med-Hoc-Net)},
  doi       = {10.1109/MedHocNet.2016.7528421},
  title     = {{Exploiting state information to support QoS in Software-Defined WSNs}},
  year      = {2016},
  url       = {http://ieeexplore.ieee.org/document/7528421/},
}
```

```
@inproceedings{Galluccio:2015b,
  author    = {Laura Galluccio and Sebastiano Milardo and Giacomo Morabito and Sergio Palazzo},
  booktitle = {2015 IEEE Conference on Computer Communications Workshops (INFOCOM WKSHPS)},
  doi       = {10.1109/INFCOMW.2015.7179322},
  title     = {{Reprogramming Wireless Sensor Networks by using SDN-WISE: A hands-on demo}},
  year      = {2015},
  url       = {http://ieeexplore.ieee.org/document/7179322/},
}
```

```
@inproceedings{Galluccio:2015a,
  author    = {Laura Galluccio and Sebastiano Milardo and Giacomo Morabito and Sergio Palazzo},
  booktitle = {2015 IEEE Conference on Computer Communications (INFOCOM)},
  doi       = {10.1109/INFOCOM.2015.7218418},
  title     = {{SDN-WISE: Design, prototyping and experimentation of a stateful SDN solution for WIreless SEnsor networks}},
  year      = {2015},
  url       = {http://ieeexplore.ieee.org/document/7218418/},
}
```
