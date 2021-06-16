---
date: 2021-03-15
title: Aquatic Toxicity Analysis with the aid of Autonomous Surface Vehicle (ASV)
linkTitle: "ASV"
tags: ["project", "ai", "environment"]
description: "Aquatic Toxicity Analysis with the aid of Autonomous Surface Vehicle (ASV)"
author: Saptarshi Sinha
github_repo: "https://github.com/cybertraining-dsc/fa20-523-312/edit/main/project/project.md"
resources:
- src: "**.{png,jpg}"
  title: "Image #:counter"
---

[![Check Report](https://github.com/cybertraining-dsc/fa20-523-312/workflows/Check%20Report/badge.svg)](https://github.com/cybertraining-dsc/fa20-523-312/actions) 
[![Status](https://github.com/cybertraining-dsc/fa20-523-312/workflows/Status/badge.svg)](https://github.com/cybertraining-dsc/fa20-523-312/actions)
Status: final, Type: Project

Saptarshi Sinha, [fa20-523-312](https://github.com/cybertraining-dsc/fa20-523-312/), [Edit](https://github.com/cybertraining-dsc/fa20-523-312/blob/main/project/project.md)

{{% pageinfo %}}

## Abstract

With the passage of time, human activities have created and contributed much to the aggrandizing problems of various forms of environmental pollution. Massive amounts of industrial effluents and agricultural waste wash-offs, that often comprise pesticides and other forms of agricultural chemicals, find their way to fresh water bodies, to lakes, and eventually to the oceanic systems. Such events start producing a gradual increase in the toxicity levels of marine ecosystems thereby perturbing the natural balance of such water-bodies. In this endeavor, an attempt will be made to analyze the various water quality metrics (viz. temperature, pH, dissolved-oxygen level, and conductivity) that are measured with the help of autonomous surface vehicles (ASV). The collected data will undergo big data analysis tasks so as to find the general trend of values for the water quality of the given region. These obtained values will then be compared with sample water quality values obtained from neighboring sources of water for ascertaining if these sample values exhibit aberration from the established values that were found earlier from the big data analysis tasks for water-quality standards. In the event, the sample data popints significantly deviate from the standard values established earlier, it can then be successfully concluded that the aquatic system in question, from which the water sample was sourced from, has been degraded and may no longer be utilized for any form of human usage, such as being used for drinking water purposes.

Contents

{{< table_of_contents >}}

{{% /pageinfo %}}

**Keywords:** toxicology, pollution, autonomous systems, surface vehicle, sensors, arduino, water quality, data analysis, environment, big data, ecosystem 

## 1. Introduction

When it comes to revolutionizing our qualities of life and improving standards, there is not another branch of science and technology that has made more impact than the myriad technological capabilities offered by the areas of Artificial Intelligence (AI) and its sub-fields involving Computer Vision, Robotics, Machine Learning, Deep Learning, Reinforcement Learning, etc. It should be borne in mind that AI was developed to allow machines/computer processors to work in the same way as the human brain works and which could make intelligent decisions at every conscious level. It was meant to help with tasks for rendering scientific applications more smarter and efficient. There are many tasks that can be performed in a far more dexterous fashion by employing smart-machines and algorithms than by involving human beings. But even more importantly, AI has also been designed to perform tasks that cannot be successfully completed by employing human beings. This could either be due to the prolonged boredom of the task itself, or a task that involves hazardous environments that cannot sustain life-forms for a long time. Some examples in this regard would involve exploring deep mines or volcanic trenches for mineral deposits, exploring the vast expanse of the universe and heavenly bodies, etc. And this is where the concept employing AI/Robotics based technology fits in perfectly for aquatic monitoring and oceanographical surveillance based applications.
 
Toxicity analysis of ecologically vulnerable water-bodies, or any other marine ecosystem for that matter, could give us a treasure trove of information regarding biodiversity, mineral deposits, unknown biophysical phenomenon, but most importantly, it could also provide meaningful and scientific information related to the degradation of the ecosystem itself. In this research endeavor, an attempt will be made to utilize aquatic Autonomous Surface Vehicle (ASV) that will be deployed in marine ecosystems and which can continue collecting data for a prolonged period of time. Such vehicles are typically embedded with different kinds of electronic sensors, that are capable of measuring physical quantities such as temperature, pH, specific conductance, dissolved oxygen level, etc. The data collected by such a system can either be over a period of time (temporal data), or it could cover a vast aquatic geographical region (spatial data). This is the procedure by which environmental organizations record and store massive amounts of data that can be analyzed to obtain useful information about the particular water body in question. Such analytical work will provide us with statistical results that can then be compared with existing sample values so as to decipher whether the water source, from where the sample was obtained, manifests normal trend of values or shows large deviations from established trends that can signify an anomaly or biodegradation of the ecosystem. The datasets used in this endeavor are provided publicly by environmental organizations in the United States, such as the US Geological Survey (USGS). While the primary goal involves conducting big data analysis tasks for the databases so as to obtain useful statistical results, a secondary goal in this project involves finding out the extent to which a particular sample of water, obtained from a specific source of water, deviates from the normal trend of values. The extent of such deviations can then give us an indication about the status of the aquatic degradation of the ecosystem in question. The data analysis framework will be made as robust as possible and in this effort, we will work with data values that are spread over multiple years and not just focused on a single year. 


## 2. Background Research and Previous Work

After reviewing the necessary background literature and previous work that has been done in this field, it can be stated that most of such endeavors focused majorly on environmental data collection with the help of sensors attached to a navigational buoy in a particular location of a water-body. Such works did not involve any significant data analysis framework and focused on particular niche areas. For instance, a particular research effort involved deploying a surface vehicle that collected data from large swaths of geographical areas in various water bodies but concentrated primarily on different algorithms employed for vehicular navigation and their relative success rates [^1]. Other research attempts focussed on even more niche areas such as study of the migration pattern exhibited by zooplanktons upon natural and aritifical irradiance [^2], and detection and monitoring of marine fauna [^3]. Although these are interesting projects and can provide us with novel information about various aspects of biological and aquatic research, such research attempts neither focused much on the data analysis portion for multiple sensory inputs (viz. temperature, pH, specific conductance, and dissolved oxygen level, which are the four most important water quality parameters) nor did they involve an intricate procedure to compare the data with sample observations so as to arrive at a suitable conclusion regarding the extent of environmental degradation of a particular water body.

As mentioned in the previous section, this research endeavor will exhaustively focus not just on the working principles and deployment of surface vehicles to collect data, but it will also involve employing deeper study towards the subject of big-data analysis of both the current data of the system in question and the past data obtained for the same aquatic profile. In this way, it would be possible to learn more about the toxicological aspects of the ecosystem in question and which can then be also applied to neighboring regions.


## 3. Choice of Data-sets

Upon exploring a wide array of available datasets, the following two data repositories were given consideration to get the required water quality based data over a particular period of time and for a particular geographical region:

1. [USGS Water Quality Data](https://waterdata.usgs.gov/nwis/qw) [^4]
2. [EPA Water Quality Data](https://www.epa.gov/waterdata/water-quality-data-download) [^5]

After going through the sample data values than can be visualized from the respective websites of USGS and EPA, the USGS datasets were chosen over the EPA datasets. This is mainly because the USGS datasets are more commensurate with the research goal of this endeavor, especially since it contains a huge array of databases that focuses on the four most important water quality data which are - temperature, pH, specific conductance, and dissolved oxygen level. Some previous work was conducted on similar USGS datasets by a particular research team [^6]. However, such work was drastically different in nature, when compared with this research attempt, since its emphasis was on a very broad perspective so as to create an overview of how to use and visualize the data from the USGS water quality portal. Besides, such work emphasizes on characterizing the seasonal variation of lake water clarity in different regions throughout the continental US, something that is very deviant from what would be addressed in this particular article which majorly involves studying environmental degradation and aquatic toxicology from the context of big data analytical tasks.

To address the questions involving existence of multiple data-sets and motivation of using multiple data-sets, we must keep in mind that the very nature of this study is based on historical trends of the nature of water-quality in a particular region from the past and to this effect, emphasis has been given to use data values from the past years as well in addition to the current year. The geographical location for this analysis was chosen to be the East Fork Whitewater River that is located at Richmond, IN (USA). The years that have been chosen in this case are 2017, 2018, 2019, and 2020. For all these years, focus would be placed on the same time-period, that spans from November 1 to November 14, for all these years so as to establish consistency and high fidelity across the borad. Having multiple data-sets in this way will help us in achieving robust data-analytical results. It would also ensure that too much focus is not given on outlier cases, that may be relevant to just a particular time and day on a given year, or an aberration in the data that may only have surfaced due to an unknown underlying phenomenon or some form of cataclysmic event from the past. Using multiple datasets would help to get a resultant data structure that is more likely to converge towards an approximate level of historical thresholds and which can then be used to find out how a current sample data-point deviates from such established trends of previous patterns.


## 4. Methodology

### 4.1 Hardware Component

Although this project focuses more on the data analysis portion than mechanical details, some information relating to the design and working principle of ASVs is provided herewith.The rough outline of an autonomous surface vehicle (ASV) in question has been perceived in Autodesk Fusion 360, which is a software package that helps creating and printing three-dimensional custom designs. A preliminary model has been designed in this software and after printing, it can be interfaced with the appropriate sensors in question. The system can be driven by an Arduino-Uno based microcontroller or even a Raspberry Pi based microprocessor, and it can comprise different types of environmental sensors that helps with collecting and offloading data to remote servers/machines. Some of these sensors can be purchased commercially from the vendor, "Atlas Scientific" [^7]. For instance, the following sensors can be used with an ASV to measure the four most important water quality parameters involving temperature, pH, dissolved oxygen level, and specific conductance values: 

* [PT-1000 Temperature sensor kit](https://atlas-scientific.com/kits/pt-1000-temperature-kit/) [^7]
* [Potential of Hydrogen (pH) sensor kit](https://atlas-scientific.com/kits/ph-kit/) [^7]
* [Dissolved Oxygen (DO) sensor kit](https://atlas-scientific.com/kits/dissolved-oxygen-kit/) [^7]
* [Conductivity K 1.0 sensor kit](https://atlas-scientific.com/kits/conductivity-k-1-0-kit/) [^7]

A very rudimentary framework of such a system has been realized in the Autodesk Fusion 360 software architecture as shown below. A two-hull framework is usually more helpful than a single hull based design since the former would help with stability issues especially while navigating through choppy waters. Figure 1 shows the design in the form of a very simplistic platform but which definitely lays down the foundation for a more complex structure for an ASV system.

![ASV from Fusion 360](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/asvdesign.png)

**Figure 1:** Nascent framework of an ASV system in Fusion 360

With the chassis framework out of the way, a careful analysis could be conducted towards the other successful components of such a vehicle so as to complete the entire build process for a fully functional prototype ASV. In essence, an ASV can be thought of being composed of certain key sub-elements. From a broad perspective, they comprise the hardware makeup, a suitable propulsion system, a sensing system, a communication system, and an appropriate source of onboard power source. The hardware makeup being out of the way, the other aspects can now be elaborated as follows:

**Propulsion System:** Primarily, the two major possibilities for propulsion systems in an ASV involve using either a single servo motor with an assortment of rudders and propellers for appropriate steering, or using two separate servo motors, one of which will drive the left-hand side of the system and the other would drive the right-hand side. The second arrangement is preferred in many scenarios as it provides with better maneuverability and control of the system as a whole. For instance, to move forward in a rectilinear fashion, both the motors would be given the same level of power. Whereas for steering the system in a particular direction, one of the motors would be assigned a lower power level than the other, thereby enabling the system to curve inwards on the side which has the motor with a lower power level. Of course, there will always be perturbations and natural disturbances that will deter the system from making these correct path changes. For this reason, a Proportional-Integral-Derivative (PID) controlled response could be augmented with the locomotion algorithms.

**Sensing System:** An ASV can have as many sensors as possible (dependent upon physical and electrical constraints of microcontroller/microprocessor) but for a study like this, an arrangement involving four different sensors needs to be integrated in the ASV which measures the four principle water quality parameters. This way, when the entire ASV system is deployed in an aquatic environment, it will be able to simultaneously provide readings for all four water-quality parameters in this case. Precisely, these water-quality parameters would be temperature, potential of hydrogen (pH), dissolved oxygen level, and specific conductance value. It should be noted in this perspective that it is possible to include even more sensors in this ASV system. However, the reason why it is generally not helpful to go beyond a certain number of sensors is primarily because of two reasons. Firstly, these parameters are important to most toxicological analysis studies [^1], and the readings provided by such a sensory system could be considered as a foundation which could provide future directions (including adding more sensors, if needed). Secondly, we should also keep in mind that the hardware system has certain constraints. In this scenario, it involves a sensory shield (that can be integrated with a microcontroller or microprocessor) which can be used for incorporating multiple sensors. But it also has a maximum of four ports for four different sensors only. Though it is possible to add multiple layers of shield on top of the others (thereby raising the capability of integrating the number of sensors to eight or even more), it leads to unnecessary bandwidth issues, memory depletion possibilities, along with an increased demand of higher power supply. These issues will especially be more consequential if we are dealing with a microcontroller that has very limited memory and power, unlike a microprocessor. Hence, the decision to stick with only a certain number of sensors is really an important one.

**Communication System:** This is possibly the most important part of the ASV system as we need to device a technique to offload the data that is collected by the vehicle back to a remote computer/server that would likely be located at a considerable distance away from the ASV. There are different options that can be considered in this regard for establishing a proper communicative functionality between the ASV and the remote computer. Some options that are typically considered involve Bluetooth, IR signals, RF signals, GPS-based system, satellite communication, etc. There are both pros and cons when it comes to using any of these different communication systems for the ASV. However, the most important metric in this case involves the maximum range the communication system could span over. Obviously, some of the options (viz. Bluetooth) would not be possible in this regard as they have a very limited communication range. Some others (viz. satellite communication systems) have a very high range but are nevertheless not feasible for small-scale research endeavors as they require too much onboard processing power to even carry out their most basic operations. Hence, a balanced approach is normally followed in these scenarios and a GPS/RF-based system is often found to be a reliable candidate for carrying out the proposed tasks of an ASV.

**Power Source:** Finally, we certainly need an onboard processing power system that can provide the required amount of power to all the functional entities housed in the ASV system. The characteristic of such a desired power source would be that it would not require frequent charging and can sustain proper ASV operations for at least five to six hours. Additionally, the weight of the power source should also not be too clumsy that might put the stability of the entire ASV system in jeopardy. It must have a suitable weight, and should also come in an appropriate shape and size such that the weight of the entire power module is evenly distributed over a large area, thereby further reinforcing the stability of the system. 


### 4.2 Software Component

With the help of the collected data from ASVs, the datasets of USGS are then prepared which meticulously tabulates all the readings from the different water sensors of the ASV. Such tabular data is made public for research and other educational purposes. In this endeavor, such datasets will be analyzed to decipher the median convergent values of the water body for the four different parameters that have been measured (i.e. temperature, pH, dissolved oxygen level, and specific conductance). The results of this data analysis task will manifest the water quality parametric values and standards for the particular aquatic ecosystem. Such a result will then be used to find out if a different water sample value sourced from a particular region deviates by a large proportion from the established standards which was obtained after analyzing the historical data from USGS for a regional source of water. The USGS website makes it easier to find data from a nearby geographical region by making it possible to enter the desired location prior to searching for water quality data in their huge databases. In this way, one can also use these databases to figure out if the water quality parameters of the particular ecological system varies wildly from a neighboring system that has almost the same geographical and ecological attributes.

The establishment of the degree of variance of the sample data from the normal standards will be carried out by deciphering the number of water quality paramteric values that are aberrant in nature. For instance, a sample value with only an aberrant pH value could be classified as "Critical Category 1" whereas, a sample value with aberrant values for pH, temperature, and specific conductance would be classified as "Critical Category 3". The aberrant nature of a particular parameter is postulated by enumerating how far the values are away from the established median data, which was obtained from the past/historical datasets. This will involve centroid-based calculations for the k-means algorithm (discussed in the next section). Such aberrant nature of a particular water quality paramteric value can also be figured out by using the context of standard deviations and quartile ranges. For instance, if the current data resides in the second quartile, it can be demarcated as being more or less consistent with previously established values. However, if it resides in the first or third quartile then it might be that the particular ecosystem has aberrant aspects, which would then need to be investigated for possible effects of outside pollutants (viz. industrial effluents, agricultural wash-off, etc.), or presence of harmful invasive species that might be altering the delicate natural balance of the ecosystem in question.

The software logic is located at this [link](https://github.com/cybertraining-dsc/fa20-523-312/blob/main/project/code/toxicologyASV.ipynb) [^8]. It has been created using the aid of Google Colaboratory platform, or simply Colab [^9]. The code has been appropriately commented and documented in such a way that it can be easily reproduced. Important instructions and vital information about different aspects of the code have been properly written down wherever necessary. The coding framework helps in corroborating the inferences and conclusions made by this research attempt, and which are described in detail in the subsequent sections. The major steps that have been followed in establishing the software logic for this big-data analytical task are discussed below.

#### 4.2.1 Data Pre-processing

**Meta-data**: As with any other instance of big data, the data obtained from the USGS website is rife with many unnecessary information. Most of these information relate to meta-data for the particular database and it also contains detailed logistical information such as location information, units used for measurement, contact information, etc. Fortunately, all these information have been bunched up nicely at the beginning of the database and they were conveniently filtered out by skipping the first thirty-four (34) rows while reading the corresponding comma separated value (csv) files.

**Extraction of required water-quality parameters (Temperature, Specific Conductance, pH, Dissolved Oxygen)**: After filtering out the meta-data, it is very essential to focus only on the relevant portion of the database which contains the required information that is needed for the data analysis tasks. In this case, if we observe carefully, we will notice that not all the columns contain the required information relating to water-quality parameters. Some of them include information such as date, time, system's unit, etc. Since these will not be required for our analysis task, we extract only those columns that contain information relating to the four primary water-quality parameters. Figure 2 displays the layout of the USGS dataset files containing all the extraneous information that are deemed unnecessary for the big data analysis task.

![database sample](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/sampledatabase.png)

**Figure 2:** Sample Database file obtained from the USGS water-quality database for the year 2017

#### 4.2.2 Attributes of the preliminary data

**Seasonal Consistency**: The preliminary data, that was pre-processed and extracted, was plotted to visualize the basic results. The data pertains to a particular duration of time in a specific seasonal time of the year, more importantly that spans the first two weeks of November for all the four years. This has been done to maintain consistency of results across the platform and to create as much as a robust framework as possible that can have high fidelity.

**Data-points as x-axis**: Additionally, it should be kept in mind that the data has already been time-stamped rigorously. More precisely, the databases that are uploaded to the USGS website have data tabulated in them that are arranged in a chronological manner. As a result, having the x-axis refer to actual data-points means the same if we had the x-axis refer to time instead. These plotted results have been provided in the next section.

**Visualization of trends**: The preliminary plotting of the data helps us to visualize the overall trends of the variation of the four important water-quality parameters. This gives an approximate idea regarding what we should normally expect from the water-quality data, the approximate maximum and minimum range of values, and it further helps in detecting any kind of outlier situations that might arise either due to the presence of artifacts, or nuisance environmental variables.

#### 4.2.3 Unsupervised learning: K-means clustering analysis ("Safe" & "Unsafe" Centroid calculation)

**General Clustering Analysis**: The concept behind any clustering based approach involves an unsupervised learning mechanism. This means that the dataset traditionally does not come labelled and the task in hand is to find patterns within the data-set based on suitable metrics. These patterns help delineate the different clusters and classify the data by assigning them to one of these clusters. This process is usually carried out by measuring the euclidean distance of each point from the "centroids" of every cluster. The resultant clusters are created in such a way that the distance within the points in a particular cluster are minimized as much as possible whereas, the corresponding distance between points from different clusters are maximized. Figure 3 summarizes this concept of clustering technique.

![clustering concept](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/clusteranalysis.png)

**Figure 3:** Concept of Clustering analysis adopted as an unsupervised learning process [^DataMining]

**K-means Classification: Centroid Calculation**: The algorithm for this step first starts with selecting a random centroid value to start with to begin the iteration process. In order to be rigorous in this regard, the initial points for centroid values were chosen to be one standard deviation away from the median values for the four water-quality parameters. More importantly, two initial centroid values were chosen that would result in two clusters, one belonging to the safe water-standard cluster and the other belonging to the unsafe category. For the safe centroid value, the point chosen was such that it was one standard deviation lower than the median values for the temperature and specific conductance parameters, whereas it was one standard deviation higher than the median values for the pH and disolved oxygen level parameters. This logic was reversed in case of the unsafe centroid starting value. The intuition behind this approach comes from the fact that a lower temperature and specific conductance value means lower degree of exothermic reactions and lower amount dissolved salts which are typically the traits of unpolluted water sources, and which also have higher pH value (that is, less acidic) and higher level of dissolved oxygen. Hence, the initial centroid value for the "safe" category was chosen in this way. For the unsafe cateory, the metrics were simply reversed.

**Iteration process**: The next steps for the centroid calculation involves creating an iteration process which will keep updating and perfecting the centroid values upon every execution of the iteration. In this case, the condition for ending the iteration involved either exceeding fifty iterations or reaching the ideal situation where the new centroid value equals the previous centroid value. In the later case, it can be mentioned that the centroid calculation has converged to a specific ideal value. Fortunately, in the case of this project, it was possible to arrive at this convergence of centroid values with not too many iteration steps. The details of this process has been explained in the coding framework with appropriate comments. 

**Assigning of Clusters**: At the end of the iteration step, we end up with the final centroid values for the safe and unsafe category. With the help of these values, we calculate the euclidean distance for every points and assign them to appropriate clusters to which they are closest to. In this way, we complete the unsupervised algorithm of clustering process for any unlabelled data that is provided to us. In this particular endeavor, we assign the value "0" for a predicted cluster indicating a safe set of water-quality values for a given point, and a value of "1" for an unsafe set of water-quality values for a given point. Figure 4 summarizes this idea behind the K-means clustering method that chiefly works as an unsupervised learning algorithm.

![k-means idea](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/kmeansclustering.png)

**Figure 4:** Concept of Clustering analysis adopted as an unsupervised learning process [^KMeans]

#### 4.2.4 Display of results & analysis of any given sample values set

In the final step, we display all the results and relevant plots for this big-data analysis task. Additionally, based on the labelled data and predicted classes for safe and unsafe water-quality standards, it will now be possible to find whether an arbitrary set of data values, that represent water-quality data for a particular region, would be classified as safe or unsafe as per this technique. This has also been shown in the results section. 

## 5. Inference

### 5.1 Analysis of extracted data and statistical information

The first preliminary set of results were analyzed to get a general idea of how the water quality paramters vary for the system in question. For the purposes of data visualization, the processed data (viewed as a data-frame in python) was first analyzed to understand the four primary water-quality parameters that are being worked upon. The data-frames for the big data sets are shown below, along with the corresponding statistical information that were evalauted for such attributes. Figure 5 shows the preliminary results that were obtained for the data visualization and statistical processing tasks.

![Preliminary results](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/prelimresults.png)

**Figure 5:** Displaying results of data visualization and statistical information for the water-quality parameters

In the above set of results, it should be worthwhile to note that temperature is measured in the celsius scale, specific conductance is measured in microsiemens per centimeter at 25 degree celsius, pH is measured in the usual standard range (between 0-14), and the level of dissolved oxygen is measured in milligrams per liter.

Next, the content of the dataset, after it is processed in the software architecture, is plotted. It displays the alteration of the values (expressed in scatter plots) of the four main water-quality parameters (viz. Temperature, Specific Conductance, pH, and Dissolved Oxygen) over the period of time that starts from November 1 to November 14 for the four years involving 2017, 2018, 2019, and 2020.

Figure 6 displays the scatter plot data for the "temperature" attribute in the year 2017.

![Temperature 2017](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/seventeentemp.png)

**Figure 6:** Scatter plot for the water-quality parameter involving "Temperature" (2017)

Figure 7 displays the scatter plot data for the "specific conductance" attribute in the year 2017.

![Conductance 2017](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/seventeencond.png)

**Figure 7:** Scatter plot for the water-quality parameter involving "Specific Conductance" (2017)

Figure 8 displays the scatter plot data for the "pH" attribute in the year 2017.

![pH 2017](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/seventeenph.png)

**Figure 8:** Scatter plot for the water-quality parameter involving "pH" (2017)

Figure 9 displays the scatter plot data for the "dissolved oxygen" attribute in the year 2017.

![Dissolved Oxygen 2017](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/seventeendox.png)

**Figure 9:** Scatter plot for the water-quality parameter involving "Dissolved Oxygen" (2017)

Figure 10 displays the scatter plot data for the "temperature" attribute in the year 2018.

![Temperature 2018](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/eighteentemp.png)

**Figure 10:** Scatter plot for the water-quality parameter involving "Temperature" (2018)

Figure 11 displays the scatter plot data for the "specific conductance" attribute in the year 2018.

![Conductance 2018](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/eighteencond.png)

**Figure 11:** Scatter plot for the water-quality parameter involving "Specific Conductance" (2018)

Figure 12 displays the scatter plot data for the "pH" attribute in the year 2018.

![pH 2018](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/eighteenph.png)

**Figure 12:** Scatter plot for the water-quality parameter involving "pH" (2018)

Figure 13 displays the scatter plot data for the "dissolved oxygen" attribute in the year 2018.

![Dissolved Oxygen 2018](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/eighteendox.png)

**Figure 13:** Scatter plot for the water-quality parameter involving "Dissolved Oxygen" (2018)

Figure 14 displays the scatter plot data for the "temperature" attribute in the year 2019.

![Temperature 2019](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/nineteentemp.png)

**Figure 14:** Scatter plot for the water-quality parameter involving "Temperature" (2019)

Figure 15 displays the scatter plot data for the "specific conductance" attribute in the year 2019.

![Conductance 2019](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/nineteencond.png)

**Figure 15:** Scatter plot for the water-quality parameter involving "Specific Conductance" (2019)

Figure 16 displays the scatter plot data for the "pH" attribute in the year 2019.

![pH 2019](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/nineteenph.png)

**Figure 16:** Scatter plot for the water-quality parameter involving "pH" (2019)

Figure 17 displays the scatter plot data for the "dissolved oxygen" attribute in the year 2019.

![Dissolved Oxygen 2019](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/nineteendox.png)

**Figure 17:** Scatter plot for the water-quality parameter involving "Dissolved Oxygen" (2019)

Figure 18 displays the scatter plot data for the "temperature" attribute in the year 2020.

![Temperature 2020](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/twentytemp.png)

**Figure 18:** Scatter plot for the water-quality parameter involving "Temperature" (2020)

Figure 19 displays the scatter plot data for the "specific conductance" attribute in the year 2020.

![Conductance 2020](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/twentycond.png)

**Figure 19:** Scatter plot for the water-quality parameter involving "Specific Conductance" (2020)

Figure 20 displays the scatter plot data for the "pH" attribute in the year 2020.

![pH 2020](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/twentyph.png)

**Figure 20:** Scatter plot for the water-quality parameter involving "pH" (2020)

Figure 21 displays the scatter plot data for the "dissolved oxygen" attribute in the year 2020.

![Dissolved Oxygen 2020](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/twentydox.png)

**Figure 21:** Scatter plot for the water-quality parameter involving "Dissolved Oxygen" (2020)


### 5.2 Centroids & Predicted Classes/Clusters

Figure 22 shows the final centroid values for the safe and unsafe water-quality standards for the year 2017. Furthermore, Figure 23 shows the predicted classes for the safe and unsafe clusters, which were calculated based on the results of the centroid values, for the same year of 2017.

![centroids for 2017](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/centroidsseventeen.png)

**Figure 22:** Safe and unsafe centroid values for the year 2017.

![clusters for 2017](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/classpredictions.png)

**Figure 23:** Predicted classes for safe ("0") and unsafe ("1") clusters for the year 2017.


### 5.3 Heatmaps for the years - 2017, 2018, 2019, and 2020

For the all the four years, heatmaps were plotted to get more information about the trend of the data. Chiefly, the heatmaps give us an empirical form of ideology relating to the degree of correlation between the different water-quality parameters in this data analysis task.

Figure 24 visualizes the heat-map and shows the relationships between the various aquatic parameters for the year of 2017.

![hmap2017](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/heatmapseventeen.png)

**Figure 24:** Heatmap for the water-quality parameters (Year - 2017)

Figure 25 visualizes the heat-map and shows the relationships between the various aquatic parameters for the year of 2018.

![hmap2018](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/heatmapeighteen.png)

**Figure 25:** Heatmap for the water-quality parameters (Year - 2018)

Figure 26 visualizes the heat-map and shows the relationships between the various aquatic parameters for the year of 2019.

![hmap2019](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/heatmapnineteen.png)

**Figure 26:** Heatmap for the water-quality parameters (Year - 2019)

Figure 27 visualizes the heat-map and shows the relationships between the various aquatic parameters for the year of 2020.

![hmap2020](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/heatmaptwenty.png)

**Figure 27:** Heatmap for the water-quality parameters (Year - 2020)


### 5.4 Analysis of sample set of values

In this portion, we test the unsupervised learning mechanism on actual sample sets of water-quality values. For this purpose, we feed the sample values to the coding framework and based on the centroids calculated for the past four years, it is able to identify whether the given water sample belong in the safe or unsafe category. Further, if it belongs in the unsafe category, the system can further inform us the degree of criticality of the water-quality degradation. This is carried out by evaluating how many water quality parametric values are beyond the normal range. Based on this analysis, a critical nature is then displayed as an output result. As an example, a critical category of "2" would signify two of the water-quality parameters were beyond the normal range of values, while the others were normal. Needless to say, higher is the critical category level, the more degraded the water source is.

Figure 28 displays the results obtained for specific sample values of water quality parameters.

![sample values test](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/sampleresults.png)

**Figure 28:** Analysis of water sample values by ascertaining the degree of degradation based on critical level 


### 5.5 Benchmark information

Finally, the benchmark analysis results are shown below for the respective tasks carried out by the coding platform. Some important facts that should be kept in mind in this regard are as follows:
- The benchmark analysis was carried out using the cloudmesh benchmark procedure in Python (executed in Google Colab). 
- A sleep-time of "5" was selected as the standard for the benchmark analysis and it has been adopted consistently for all the other benchmark calculations.
- The time values for the different benchmark results were not rounded off in this case as it was both important and interesting to know the minute differences between the different kinds of tasks that were carried out in this regard. It should be noted that the final benchmark value is exceptionally high since this step involves the part where the human user inputs the sample values for ascertaining the safety standard for a water source.

Figure 29 shows the benchmark results that were obtained for specific sections in the coding framework.

![benchmark results](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/bmresults.png)

**Figure 29:** Benchmark results for all the tasks that were carried out for this big data analysis task using Google Colab


## 6. Conclusion

This research endeavor implements a big data analysis framework for analyzing toxicity of aquatic systems. It is an attempt where hardware and software meet together to give reliable results, and on the basis of which we are able to design an elaborate mechanism that can analyze other sample water sources and provide decisions regarding its degradation. Although the endeavor carried out in this example might not involve a plethora of high-end applications or intricate logic frameworks, it still provides a very decent foundational approach for carrying out toxicological analysis for water sources. Most importantly, it should be noted that the results obtained for sample values correspond to what we would normally expect for polluted and non-polluted sources of water. For instance, it was found that water sources with high values of specific conductance were categorized in the "unsafe" category which is to be expected since a high conductance value typically signifies the presence of dissolved salts and ions in the water source, which normally indicates that effluents or agricultural run-off might have made its way to the water source. Additionally, it was also found out that water samples with high values of dissolved oxygen levels were categorized in the "safe" category which is certainly true based on biological postulates.

Of course, a more diverse array of data coupled with more scientific and enhanced ASV systems would have probably provided us with even better results. But as indicated earlier, this research endeavor provides a pragmatic foundational approach to conducting this kind of big data analytical work. We can build up on the logic presented in this endeavor to come up with even more advanced and robust version of toxicological analysis tasks.


## 7. Acknowledgements

The author would like to thank Dr. Geoffrey Fox, Dr. Gregor von Laszewski, and the associate instructors in the *FA20-BL-ENGR-E534-11530: Big Data Applications* course (offered in the Fall 2020 semester at Indiana University, Bloomington) for their continued assistance and suggestions with regard to exploring this idea and also for their aid with preparing the various drafts of this article.

## 8. References

[^1]: Valada A., Velagapudi P., Kannan B., Tomaszewski C., Kantor G., Scerri P. (2014) Development of a Low Cost Multi-Robot Autonomous Marine Surface Platform. In: Yoshida K., Tadokoro S. (eds) Field and Service Robotics. Springer Tracts in Advanced Robotics, vol 92. Springer, Berlin, Heidelberg. <https://doi.org/10.1007/978-3-642-40686-7_43>

[^2]: M. Ludvigsen, J. Berge, M. Geoffroy, J. H. Cohen, P. R. De La Torre, S. M. Nornes, H. Singh, A. J. Sørensen, M. Daase, G. Johnsen, Use of an Autonomous Surface Vehicle reveals small-scale diel vertical migrations of zooplankton and susceptibility to light pollution under low solar irradiance. Sci. Adv. 4, eaap9887 (2018). <https://advances.sciencemag.org/content/4/1/eaap9887/tab-pdf>

[^3]: Verfuss U., et al., (2019, March). A review of unmanned vehicles for the detection and monitoring of marine fauna. Marine Pollution Bulletin, Volume 140, Pages 17-29. Retrieved from <https://doi.org/10.1016/j.marpolbul.2019.01.009>

[^4]: USGS Water Quality Data, Accessed: Nov. 2020, <https://waterdata.usgs.gov/nwis/qw>

[^5]: EPA Water Quality Data, Accessed Nov. 2020, <https://www.epa.gov/waterdata/water-quality-data-download>

[^6]: Read, E. K., Carr, L., De Cicco, L., Dugan, H. A., Hanson, P. C., Hart, J. A., Kreft, J., Read, J. S., and Winslow, L. A. (2017), Water quality data for national‐scale aquatic research: The Water Quality Portal, Water Resour. Res., 53, 1735– 1745, doi:10.1002/2016WR019993. <https://agupubs.onlinelibrary.wiley.com/doi/epdf/10.1002/2016WR019993>

[^7]: Atlas Scientific team. Atlas Scientific Environmental Robotics. Retrieved from <https://atlas-scientific.com/>

[^8]: Sinha, Saptarshi. (2020) A Big-data analysis framework for Toxicological Study. Retrieved from <https://github.com/cybertraining-dsc/fa20-523-312/blob/main/project/code/toxicologyASV.ipynb>

[^9]: Google Colaboratory team. Google Colaboratory. Retrieved from <https://colab.research.google.com/>

[^DataMining]: Tan, Steinback, Kumar (2004, April). Introduction to Data Mining, Lecture Notes for Chapter 8, Page 2. Accessed: Nov. 2020, <https://www-users.cs.umn.edu/~kumar001/dmbook/dmslides/chap8_basic_cluster_analysis.pdf>

[^KMeans]: Alan J. (2019, November). K-means: A Complete Introduction. Retrieved from <https://towardsdatascience.com/k-means-a-complete-introduction-1702af9cd8c>
