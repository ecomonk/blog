---
layout: post
title: The Remote Sound Recording System (RS²) - A Low-Cost Acoustic Recorder for Bioacoustics Research (2015) with Remote Controlling Capabilities 
categories: [Sound, Rabpberry , IOT , NVRAM , Bioacoustics]
---
 

![](/images/rs2_model.jpg)
 
## Introduction

For centuries, scientists have recognized the importance of documenting human, animal, and environmental sounds. The field of bioacoustics has seen remarkable growth in recent decades, largely driven by advancements in recording and analysing acoustic signals. The introduction of digital recording, data storage, and analysis technologies in the 1980s revolutionised the field, making it more accessible to researchers. Gone are the days when bulky equipment and limited recording duration hindered studies. Today, researchers are able to explore the vast possibilities of bioacoustics research thanks to the accessibility, affordability, and extended recording capabilities of modern equipment.

**Acoustic** recorders play a vital role in terrain & marine bioacoustics research. However, existing devices are often expensive and lack self-calibration capabilities, which are crucial for obtaining high-quality measurements. Moreover, proprietary software in these devices can be inflexible and involve unknown processing steps. To address these limitations, a team of researchers has developed a miniature low-cost acoustic recorder called the Remote Sound Recording System (RS²). This innovative system incorporates open-source hardware and software, providing researchers with greater flexibility and control over their recordings.

## Importance of Bioacoustics Research:

Bioacoustics has revolutionised our understanding of evolution, taxonomy, wildlife conservation, and animal physiology. Birds and invertebrates produce territorial songs, bats use ultrasound to detect prey, and elephants use infrasound for communication. The unique calls and songs of different species convey valuable information about their biology, behaviour, and ecology. Acoustic recordings serve as a treasure repository of data, revealing insights into individuals, populations, and the environment. The ability to capture ecological sounds has opened up new avenues for research, enabling studies on species presence, animal movements, and vocal individuality.

## The Need for a Low-Cost Open-Source Acoustic Recorder

In the field of bioacoustics, remotely operated or handheld devices are commonly used to record ecological sounds. While automated systems that record continuously or in response to acoustic triggers have gained popularity, they often come with a hefty price tag. For large-scale studies or research involving cryptic or elusive species, the cost of deploying a significant number of commercial recording units becomes prohibitive. Although inexpensive tablet-based systems have emerged, they often contain unnecessary hardware and software, limiting their suitability for bioacoustic research.

## Introducing the RS² - A Game-Changer in Bioacoustics Research:

Recognizing the need for a low-cost, customizable acoustic recorder, we few at Livares were on paper writing up & researching how to develop a low cost product 

Concluding to the Creation of  Remote Sound Recording System (RS²). This system features a miniature design and incorporates both open-source hardware and software. At the core of the RS² is the Raspberry Pi, a credit-card-sized computer known for its versatility and low power consumption.

The RS² system captures audible sound up to 22 kHz for extended periods without requiring manual intervention. It also boasts the ability to record audio up to a Nyquist frequency of 96 kHz, ensuring high-resolution recordings. The RS² is easy to build and operate, utilising affordable hardware and readily available software components. Its compact size allows researchers to transport and deploy the system effortlessly in remote locations, eliminating the need for cumbersome recording equipment.

## Goals

The primary goals of the RS² system are as follows:

1.  Low Power Consumption: The RS² is designed to minimise power consumption while maintaining high-quality recording capabilities.
2.  Compact Size: The system is built to be portable and easily held in the palm of one's hand, allowing researchers to carry it to remote locations conveniently.
3.  Weatherproof: The RS² is constructed with weatherproof materials, enabling its deployment in various environmental conditions.
4.  Customizable: Researchers can customise the RS² system to meet their specific recording requirements, ensuring flexibility and adaptability.
5.  Cost-Effectiveness: By utilising inexpensive hardware and freely available software, the RS² offers a cost-effective alternative to traditional acoustic recorders.

##  System Overview

The RS² system is built around the Raspberry Pi, a credit-card-sized computer that serves as the core of the system. Raspberry Pi's open-source nature, compact size, and low power consumption make it an ideal choice for the RS². The system incorporates a high-sensitive microphone, a Wolfson sound processor for data conversion, and an RTC (Real-Time Clock) module for accurate timekeeping.

##  Challenges and Solutions

During the development of the RS² system, several challenges were encountered, and innovative solutions were devised:

1.  Power Management: To minimise power consumption, the RS² system avoids using high-power devices like relays. Additionally, internet connectivity is scheduled to optimise data usage.
2.  Volatile Memory Issue: The RS² system overcame the issue of volatile memory by utilising the NV SRAM (Non-Volatile Static Random-Access Memory) available in the RTC module, ensuring that the custom automated time remains intact even after MC resets.
3.  Internet Time & Config Synchronisation: The RS² system utilises NTP (Network Time Protocol) to synchronise the RTC module with internet time servers, ensuring accurate timestamps for the recordings and it has in built NV SRAM for clock and the deice can be tuned from the cloud using cloud config that will be automatically downloaded and applied once the device connected to network , this way remote configs can be updated to the recorder and parameters can be updated remotely  .
4.  Waterproof Enclosure: A waterproof enclosure was constructed using a suitable "wifi antenna box" that met the system's requirements, providing protection against environmental elements.

##  System Functioning

In operation, the RS² system captures surrounding sounds through a highly sensitive microphone. The captured sound is then boosted and converted to electronic digital data by the Wolfson sound processor. The Raspberry Pi processes and stores the digital data, which is subsequently uploaded to a storage server.

Team : @Livares    
  
*   Rineez Ahmed – Principal Designer, Livares Labs
*   Pratheesh - Embedded Engineer 
*   Syan Whislor – Developer, Livares Labs
*   Govind Raveendran – Developer, Livares Labs

##  Conclusion

The Remote Sound Recording System (RS²) offers a low-cost, open-source solution for bioacoustics research. With its compact size, low power consumption, and customizable features, the RS² empowers researchers to conduct high-quality acoustic recordings in remote environments. By addressing the limitations of existing acoustic recorders, the RS² opens up new possibilities for studying and understanding the rich biodiversity and ecological dynamics through sound.

[https://web.archive.org/web/20221130012647/https://blog.livares.com/livares-labs-project-the-remote-sound-recording-system-rs%C2%B2/](https://web.archive.org/web/20221130012647/https://blog.livares.com/livares-labs-project-the-remote-sound-recording-system-rs%C2%B2/)


