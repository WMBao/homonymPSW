# homonymPSW

--- PSW with typing patterns --- implemented in an instruction authentication mechanism in Smart Home networks


## Introduction

We apply a PSW verification method with a ML based classifier for lower false-positive rates. 
The typing dynamics are integrated to enhance security. 
A simple Android APP is developed for recording not only the typed PSWs but also the typing dynamics. 
Weka is used for comparing and selecting a classifier with ideal performance and acceptable complexity.

## Background

Nowadays, Smart Home has gained attentions among researchers in recent years due to the growth in the domain of Internet of Things (IoT). 
Smart Home networks are becoming more and more complex. 

Devices within a Smart Home usually need to have access to the Internet. 
Existing architectures include Direct Internet Access (DIA) and Gateway-based Internet Access (GIA).
Concentrating on the GIA architecture, there are many vulnerabilities that can be leveraged by malicious attacks.

Shahbaz et al. (2007) proposed a user authentication method using a RBF based neural network in Smart Home networks.

![Missing Image](https://github.com/WMBao/homonymPSW/blob/master/image/RBF-NN.png)


## PSW with typing dynamics

We collect the time series for PSWs with typing dynamics via a simple Android APP.
The APP is developed by my Group mate Kai Zhang, a first-year postgraduate student from BISTU.
Its UI is as follows.

![Missing Image](https://github.com/WMBao/homonymPSW/blob/master/image/UI.jpg)

The time series data are collocted and organized in .CSV files.

![Missing Image](https://github.com/WMBao/homonymPSW/blob/master/image/TS.jpg)

For the purpose of comparison, we create two datasets, one with typing patterns and the other without, as in ./data folder.


## Results

We conduct our experiments on our datasets with Weka.

ML based PSW verifications are demonstrated to enjoy high TPRs and Precisions, with less vulnerability of registered PSW data leakage. 

![Missing Image](https://github.com/WMBao/homonymPSW/blob/master/image/R1.jpg)

Experiments on PSWs with typing dynamics give even better results in FPRs. 
Utilizing PSWs with typing dynamics can prevent unwelcome users who know the PSW.

![Missing Image](https://github.com/WMBao/homonymPSW/blob/master/image/R2.jpg)

![Missing Image](https://github.com/WMBao/homonymPSW/blob/master/image/R3.jpg)
