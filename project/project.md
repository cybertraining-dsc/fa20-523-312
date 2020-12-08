# Aquatic Toxicity Analysis with the aid of Autonomous Surface Vehicle (ASV)

- [x] Please use references instead of using URLs to cite the work. (Response: Appropriate references have been incorporated.) 
- [x] Benchmark the separate parts of your analysis (Response: Addressed in the code, results displayed in section 5.5) 
- [x] verify if you need time on the x axis, datapoints would not allow to relate the points if they are gathered in different time intervals. THis has to be clarified while revieing the original data, (Response: Explained in section 4.2.2.) 
- [x] some plots seem only to be distinguished by the plotstyle but may not be content different. PLease verify (Response: Addressed in the "Inference" section)
- [x] Extension for project granted till last day of regular semester in December (Response: Not required.) 
- [x] modification of report beyond that granted and expected according to author. (Response: Not required.) 

[![Check Report](https://github.com/cybertraining-dsc/fa20-523-312/workflows/Check%20Report/badge.svg)](https://github.com/cybertraining-dsc/fa20-523-312/actions) 
[![Status](https://github.com/cybertraining-dsc/fa20-523-312/workflows/Status/badge.svg)](https://github.com/cybertraining-dsc/fa20-523-312/actions)
Status: in progress, Type: Project

Saptarshi Sinha, [fa20-523-312](https://github.com/cybertraining-dsc/fa20-523-312/), [Edit](https://github.com/cybertraining-dsc/fa20-523-312/blob/main/project/project.md)

{{% pageinfo %}}

## Abstract

With the passage of time, human activities have created and contributed much to the aggrandizing problems of various forms of environmental pollution. Massive amounts of industrial effluents and agricultural waste wash-offs, that often comprise pesticides and other forms of agricultural chemicals, find their way to fresh water bodies, to lakes, and eventually to the oceanic systems. Such events start producing a gradual increase in the toxicity levels of marine ecosystems thereby perturbing the natural balance of such water-bodies. In this endeavor, an attempt will be made to measure the various water quality metrics (viz. temperature, pH, dissolved-oxygen level, and conductivity) with the help of an autonomous surface vehicle (ASV). This collected data will then be analyzed to ascertain if these values exhibit aberration from the established values that are found from USGS and EPA databases for water-quality standards. In the event, the collected data significantly deviates from the standard values of unpolluted sources in nearby geographical areas, that are obtained from the above databases, it can be concluded that the aquatic system in question has been degraded and may no longer be utilized for any form of human usage, such as being sourced for drinking water.

Contents

{{< table_of_contents >}}

{{% /pageinfo %}}

**Keywords:** toxicology, pollution, autonomous systems, surface vehicle, sensors, arduino, water quality, data analysis, environment, big data, ecosystem 

## 1. Introduction

When it comes to revolutionizing our qualities of life and improving standards, there is not another branch of science and technology that has made more impact than the myriad technological capabilities offered by the areas of Artificial Intelligence (AI) and its sub-fields involving Computer Vision, Robotics, Machine Learning, Deep Learning, Reinforcement Learning, etc. It should be borne in mind that AI was developed to allow machines/computer processors to work in the same way as the human brain works and which could make intelligent decisions at every conscious level. It was meant to help with tasks for rendering scientific applications more smarter and efficient. There are many tasks that can be performed in a far more dexterous fashion by employing smart-machines and algorithms than by involving human beings. But even more importantly, AI has also been designed to perform tasks that cannot be successfully completed by employing human beings. This could either be due to the prolonged boredom of the task itself, or a task that involves hazardous environments that cannot sustain life-forms for a long time. Some examples in this regard would involve exploring deep mines or volcanic trenches for mineral deposits, exploring the vast expanse of the universe and heavenly bodies, etc. And this is where the concept employing AI/Robotics based technology fits in perfectly for aquatic monitoring and oceanographical surveillance based applications.
 
Toxicity analysis of ecologically vulnerable water-bodies, or any other marine ecosystem for that matter, could give us a treasure trove of information regarding biodiversity, mineral deposits, unknown biophysical phenomenon, but most importantly, it could also provide meaningful and scientific information related to the biodegradation of the ecosystem itself. In this research project, an attempt will be made to design a simple foundation of an aquatic Autonomous Surface Vehicle (ASV) that will be deployed in marine ecosystems. Such a vehicle would be embedded with different kind of electronic sensors, that are capable of measuring physical quantities such as temperature, pH, conductance, dissolved oxygen level, etc. The data collected by such a system can either be over a period of time (temporal data), or it could cover a vast aquatic geographical region (spatial data). This data will then be compared with existing datasets that are made publicly available by various environmental organizations in the United States, most importantly the Environmental Protection Agency (EPA) and the US Geological Survey (USGS). A comparative data analysis task between the data collected by the ASV and the vast array of environmental data that are made available from these agencies can then give us an indication about the status of the aquatic degradation of the ecosystem in question by measuring the extent to which the current data deviates from relevant historical data trends. 


## 2. Background Research and Previous Work

After reviewing the necessary background literture and previous work that has been done in this field, it can be stated that most of such endeavors focussed majorly on continuous environmental data collection with the help of sensors attached to a stationary buoy in a particular location of a water-body. Some of the other endeavors did involve deploying a non-stationary vehicle that collected data from large swaths of geographical areas in various water bodies [^1]. Other research attempts focussed on niche areas such as study of the migration pattern exhibited by zooplanktons upon natural and aritifical irradiance [^2], and detection and monitoring of marine fauna [^3]. However, neither did such attempts focus much on the data analysis portion for multiple sensory input(s) nor did it involve an intricate procedure to compare the collected data with historical trends so as to arrive at a suitable conclusion regarding the extent of environmental degradation.

As mentioned in the previous section, this research project will exhaustively focus not just on the data-collection portion by a non-stationary vehicle, but it will also involve employing deeper study towards the subject of big-data analysis of both the current data of the system in question and the past data obtained for similar aquatic profiles. In this way, it would be possible to learn more about the toxicological aspects of the ecosystem in question.


## 3. Choice of Data-sets

Upon exploring a wide array of available datasets, the following data repositories were chosen to get the required water quality based data over a particular period of time and for a particular geographical region:

1. [USGS Water Quality Data](https://waterdata.usgs.gov/nwis/qw) [^4]
2. [EPA Water Quality Data](https://www.epa.gov/waterdata/water-quality-data-download) [^5]

The USGS dataset is very commensurate with the research goal of this endeavor and hence, focus will be put more on the USGS dataset over the EPA dataset. Some previous work was conducted on this USGS dataset by a particular research team [^6]. However, the emphasis of such work was done from a very broad perspective so as to create an overview of how to use and visualize the data from the USGS water quality portal. Besides, such a work emphasizes on characterizing the seasonal variation of lake water clarity in different regions throughout the continental US, something that is very deviant from what would be addressed in this particular article which majorly involves environmental degradation and toxicology analysis using an autonomous surface vehicle.

To address the questions involving existence of multiple data-sets and motivation of using multiple data-sets, we must keep in mind that the very nature of this study is based on historical trends of the nature of water-quality in a particular region from the past and how it relates to the current situation. Because of these reasons, multiple data-sets will be referred to from multiple sources so as to achieve robust data-analytical results. This would ensure that too much focus is not given on outlier cases, that may be relevant to just a particular geographical region or an aberration in the data that may only have arisen due to an unknown underlying phenomenon or some form of cataclysmic event from the past. Using multiple datasets from different sources would help to get a resultant data structure that is more likely to converge towards an approximate level of historical thresholds and which can then be used to find out how the current observed data deviates from such previous patterns.


## 4. Methodology

### 4.1 Hardware Component

The rough outline of the autonomous surface vehicle (ASV) in question has been perceived in the Autodesk Fusion 360 software model. A preliminary model has been designed in this software so as to 3D print the system. It will then be interfaced with the appropriate sensors in question. Then system will be driven by an Arduino-Uno based microcontroller, and it will have different types of environmental sensors that will collect and log data. These sensors have been purchased from the vendor, "Atlas Scientific" [^7]. As of now, the sensors that have been chosen for this ASV are as follows: 

* [PT-1000 Temperature sensor kit](https://atlas-scientific.com/kits/pt-1000-temperature-kit/) [^7]
* [Potential of Hydrogen (pH) sensor kit](https://atlas-scientific.com/kits/ph-kit/) [^7]
* [Dissolved Oxygen (DO) sensor kit](https://atlas-scientific.com/kits/dissolved-oxygen-kit/) [^7]
* [Conductivity K 1.0 sensor kit](https://atlas-scientific.com/kits/conductivity-k-1-0-kit/) [^7]

A very rudimentary framework of the system has been realized in the Autodesk Fusion 360 software architecture as shown below. The design provided below is a very simplistic platform but which will lay the foundation of the final structure of the system (see Figure 1).

![ASV from Fusion 360](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/asvdesign.png)

**Figure 1:** Nascent framework of the ASV system in Fusion 360

With the chassis framework out of the way, a careful analysis was conducted towards the successful developmental work to be done to complete the build process for a fully functional prototype ASV. In essence, an ASV can be thought of being composed of certain key sub-elements. From a broad perspective, they comprise the hardware makeup, a suitable propulsion system, a sensing system, a communication system, and an appropriate source of onboard power source. The hardware makeup being out of the way, the other aspects can now be elaborated as follows:

**Propulsion System:** The two possibilities that was considered in this regard involve using either a single servo motor with an assortment of rudders and propellers for appropriate steering, or using two separate servo motors, one of which will drive the left-hand side of the system and the other would drive the right-hand side. The second arrangement is preferred in this regard as it provides with better maneuverability and control of the system. For instance, to move forward in a rectilinear fashion, both the motors would be given the same level of power. Whereas for steering the system in a particular direction, one of the motors would be assigned a lower power level than the other, thereby enabling the system to curve inwards on the side which has the motor with a lower power level. Of course, there will always be perturbations and natural disturbances that will deter the system from making these correct path changes. For this reason, a Proportional-Integral-Derivative (PID) controlled response would be augmented for the locomotion algorithm.

**Sensing System:** As discussed previously, an arrangement involving four different sensors will be integrated in the ASV. This way, when the entire ASV system is deployed in an aquatic environment, it will be able to simultaneously provide readings for all four water-quality parameters in this case. Precisely, these water-quality parameters would be temperature, potential of hydrogen (pH), dissolved oxygen level, and specific conductance value. It should be noted in this perspective that it is possible to include even more sensors in this ASV system. However, the reason why it was not necessary to go beyond these four sensor types is primarily because of two reasons. Firstly, these parameters are important to most toxicological analysis studies [^1] and the readings provided by such a sensory system could be considered as a foundation which could provide future directions (including adding more sensors, if needed). Secondly, we should also keep in mind that the hardware system has certain constraints. In this scenario, it involves a sensory shield (that can be integrated with the Arduino microcontroller) that is being used but which has a maximum of four ports for four different sensors only. Though it is possible to add another layer of shield on top of the current one (thereby raising the capability of integrating the number of sensors to eight), it adds unnecessary bandwidth issues, memory depletion possibilities, along with an increased demand of higher power supply. These issues will especially be more consequential in this case as we are dealing with a microcontroller that has limited memory and power, unlike a microprocessor. Hence, the decision to stick with four sensors only was made.

**Communication System:** This is possibly the most important part of the ASV system as we need to device a technique to offload the data that is collected by the vehicle back to a remote computer/server that would likely be located at a considerable distance away from the ASV. There are different options that have been considered in this regard for establishing a proper communicative functionality between the ASV and the remote computer. Some options that have been considered involved Bluetooth, IR signals, RF signals, GPS-based system, satellite communication, etc. There are both pros and cons when it comes to using any of these different communication systems for the ASV. However, the most important metric in this case involves the maximum range the communication system could span over. Obviously, some of the options (viz. Bluetooth) would not be possible in this regard as they have a very limited communication range. Some others (viz. satellite communication systems) have a very high range but were nevertheless found unsuitable for this endeavor as they required too much onboard processing power to even carry out their most basic operations. Hence, a balanced approach was followed in this scenario and a GPS/RF-based system was eventually chosen as the most appropriate candidate for carrying out the proposed tasks of the ASV.

**Power Source:** Finally, we need an onboard processing power system that can provide the required amount of power to all the functional entities housed in the ASV system. The characteristic of such a desired power source would be that it would not require charging often and can sustain proper ASV operations for at least five to six hours. Additionally, the weight of the power source should also not be too clumsy that might put the stability of the entire ASV system in jeopardy. It must have a suitable weight, and should also come in an appropriate shape and size such that the weight of the entire system is evenly distributed over a large area, thereby further reinforcing the stability of the system. 


### 4.2 Software Component

After the data has been collected by the ASV either on a temporal scale (over a period of time) or a spatial scale (over a geographical area), it will then be analyzed to decipher the median convergent values of the water body for the four different parameters that have been measured (i.e. temperature, pH, dissolved oxygen level, and conductivity). The results of this data analysis task will then be used to find out if such water quality parametric values manifested by the aquatic ecosystem in question deviates by a large proportion from the other result that is obtained after analyzing the historical data from USGS for a nearby polluted/unpolluted source of water. The USGS website make it easier to find data from a nearby geographical region by making it possible to enter the desired location prior to searching for water quality data in their huge databases. In this way, it can also be used to figure out if the water quality parameters of the particular ecological system varies wildly from a neighboring system that has almost the same geographical and ecological attributes.

The establishment of the degree of variance of the data from the historical data will be carried out by documenting the particular quartile range that the current data lies in with respect to the median data that is obtained from the past/historical datasets. For instance, if the current data resides in the second quartile, it can be demarcated as being more or less consistent with previously established values. However, if it resides in the first or third quartile then it might will that the system has aberrant aspects which might need to be investigated for possible levels of outside pollutants (viz. industrial effluents, agricultural wash-off, etc.), or presence of harmful invasive species that might be altering the delicate natural balance of the ecosystem in question.

The software logic can be located at this [link](https://github.com/cybertraining-dsc/fa20-523-312/blob/main/project/code/toxicologyASV.ipynb) [^8]. It has been created using the aid of Google Colaboratory platform, or simply Colab [^9]. Furthermore, the code has been appropriately commented and documented in such a way that it can be easily reproduced. Important instructions and vital information about different aspects of the code have been properly written down wherever necessary. The coding framework helps in postulating the inferences and conclusions of this research attempt, and which are described in detail in the subsequent sections. The major steps that has been followed in establishing the software logic for this big-data analysis task have been discussed below.

#### 4.2.1 Data Pre-processing

**Meta-data**: As with any other instance of big data, the data obtained from the USGS website is rife with many unnecessary information. Most of these information relate to meta-data for the particular database and it also contains detailed logistical information such as location information, units used for measurement, contact details, etc. Fortunately, all these information have been bunched up nicely at the beginning of the database and they were conveniently filtered out by skipping the first thirty-four rows while reading the corresponding comma separated value (csv) files.

**Extraction of four water-quality parameters (Temperature, Specific Conductance, pH, Dissolved Oxygen level)**: After filtering out the meta-data, it is also essential to focus on the relevant portion of the database which contains the information that we are looking for. In this case, if we observe carefully, we will notice that not all the columns contain the required information relating to water-quality parameters. Some of them include information such as date, time, system's unit, etc. Since these will not be required for our analysis task, we extract only those columns that contain information relating to the four primary water-quality parameter.

A sample file has been provided below that displays all the information contained in the USGS database files.

![database sample](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/sampledatabase.png)

**Figure 2:** Sample Database file obtained from the USGS water-quality database for the year 2017

#### 4.2.2 Analysis of preliminary statistical information

**Seasonal Consistency**: The preliminary data, that was pre-processed and extracted, was plotted. The data pertains to a particular duration of time in a specific seasonal time of the year, more importantly that spans the first two weeks of November for all the four years. This has been done to maintain consistency of results across the platform and to create as much as a robust framework as possible that can have high fidelity.

**Data-points as x-axis**: Additionally, it should be kept in mind that the data was already time-stamped rigorously. More precisely, the databases that are uploaded to the USGS website have data tabulated in them that are arranged in a chronological manner. As a result, having the x-axis refer to actual data-points means the same if we had the x-axis refer to time instead. These plotted results have been provided in the next section.

**Visualization of trends**: The preliminary plotting of the data helps us to visualize the overall trends of the variation of the four important water-quality parameters. This gives an approximate idea regarding what we should normally expect from the water-quality data, the approximate maximum and minimum range of values, and it further helps in detecting any kind of outlier/aberrant situations that might arise either due to the presence of artifacts, or nuisance environmental variables.

#### 4.2.3 Unsupervised learning: K-means clustering analysis ("Safe" & "Unsafe" Centroid calculation)

**General Clustering Analysis**: The concept behind any clustering based approach involves an unsupervised learning mechanism. This means that the dataset traditionally does not come labelled and the task in hand is to find patterns within the data-set based on suitable metrics. These patterns help delineate the different clusters and classify the data by assigning them to one of the clusters. This process is usually carried out by measuring the euclidean distance of each point from the "centroids" of every cluster. The resultant clusters are created in such a way that the distance within the points in a particular cluster are minimized whereas, the corresponding distance between points from different clusters are maximized. This concept can be summarized by the figure below.

![clustering concept](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/clusteranalysis.png)

**Figure 3:** Concept of Clustering analysis adopted as an unsupervised learning process [^10]

**K-means Classification: Centroid Calculation**: The algorithm for this step first starts with selecting a random centroid value to start with to begin the iteration process. In order to be rigorous in this regard, the initial points for centroid values were chosen to be one standard deviation away from the median values for the four water-quality parameters. More importantly, two initial centroid values were chosen that would result in two clusters, one belonging to the safe water-standard cluster and the other belonging to the unsafe category. For the safe centroid value, the point chosen was such that it was one standard deviation lower than the median values for the temperature and specific conductance parameters, whereas it was one standard deviation higher than the median values for the pH and disolved oxygen level parameters. This logic was reversed in case of the unsafe centroid starting value. This can be summarized by the following code-excerpt.

'''
mu_safe = [(t_med - (1*std[0])), (c_med - (1*std[1])), (p_med + (1*std[2])), (d_med + (1*std[3]))]
mu_unsafe = [(t_med + (1*std[0])), (c_med + (1*std[1])), (p_med - (1*std[2])), (d_med - (1*std[3]))]
'''

**Iteration process**: The next steps for the centroid calculation involves creating an iteration process which will keep updating and perfecting the centroid values upon every execution of the iteration. In this case, the condition for ending the iteration involved either exceeding fifty iterations or reaching the ideal situation where the new centroid value equals the previous centroid value. In the later case, it can be mentioned that the centroid calculation has converged to a specific ideal value. Fortunately, in the case of this project, it was possible to arrive at this convergence of centroid values with not too many iteration steps. The details of this process has been explained in the coding framework. 

**Assigning of Clusters**: At the end of the iteration step, we end up with the centroid values and with the help of these values we calculate the euclidean distance for every points and assign them to appropriate clusters to which they are closest to. In this way, we complete the unsupervised algorithm of clustering process for any unlabelled data that is provided to us. In this particular endeavor, we assign the value "0" for a predicted cluster indicating a safe set of water-quality values for a given point, and a value of "1" for an unsafe set of water-quality values for a given point. The following figure summarizes this idea.

![k-means idea](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/kmeansclustering.png)

**Figure 4:** Concept of Clustering analysis adopted as an unsupervised learning process [^11]

#### 4.2.4 Display of results & analysis of any given sample values set

In the final step, we display all the results and plotting information for this big-data analysis task. Additionally, based on the labelled data and predicted classes for safe and unsafe water-quality standards, it will now be possible to find whether an arbitrary set of data values, that represents water-quality data for the surrounding region, would be classified as safe or unsafe as per this technique. This has also been shown in the results section. 

## 5. Inference

### 5.1 Plotting of extracted data

The first preliminary set of results are displayed below. To get a better idea, the processed data (viewed as a data-frame in python) was first analyzed to understand the four primary water-quality parameters that are being worked upon. The data-frame for one of the big data sets is shown below, along with the median values that were evalauted for the respective parameters.

![Preliminary results](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/prelimresults.png)

**Figure 5:** First set of preliminary output results (in python data-frame) and median values for the four water-quality parameters

In the above set of results, it should be worthwhile to note that temperature is measured in the celsius scale, specific conductance is measured in microsiemens per centimeter at 25 degree celsius, pH is measured in the usual standard range (between 0-14), and the level of dissolved oxygen is measured in milligrams per liter.

Next, the content of the dataset, after it is processed in the software architecture, is shown and it displays the alteration of the values (expressed in scatter plots) of the four main water-quality parameters (viz. Temperature, Specific Conductance, pH, and Dissolved Oxygen) over the period of time that starts from November 1 to November 14 for the four years involving 2017, 2018, 2019, and 2020.

![Temperature 2017](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/seventeentemp.png)

**Figure 6:** Scatter plot for the water-quality parameter involving "Temperature" (2017)

![Conductance 2017](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/seventeencond.png)

**Figure 7:** Scatter plot for the water-quality parameter involving "Specific Conductance" (2017)

![pH 2017](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/seventeenph.png)

**Figure 8:** Scatter plot for the water-quality parameter involving "pH" (2017)

![Dissolved Oxygen 2017](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/seventeendox.png)

**Figure 9:** Scatter plot for the water-quality parameter involving "Dissolved Oxygen" (2017)

![Temperature 2018](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/eighteentemp.png)

**Figure 10:** Scatter plot for the water-quality parameter involving "Temperature" (2018)

![Conductance 2018](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/eighteencond.png)

**Figure 11:** Scatter plot for the water-quality parameter involving "Specific Conductance" (2018)

![pH 2018](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/eighteenph.png)

**Figure 12:** Scatter plot for the water-quality parameter involving "pH" (2018)

![Dissolved Oxygen 2018](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/eighteendox.png)

**Figure 13:** Scatter plot for the water-quality parameter involving "Dissolved Oxygen" (2018)

![Temperature 2019](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/nineteentemp.png)

**Figure 14:** Scatter plot for the water-quality parameter involving "Temperature" (2019)

![Conductance 2019](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/nineteencond.png)

**Figure 15:** Scatter plot for the water-quality parameter involving "Specific Conductance" (2019)

![pH 2019](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/nineteenph.png)

**Figure 16:** Scatter plot for the water-quality parameter involving "pH" (2019)

![Dissolved Oxygen 2019](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/nineteendox.png)

**Figure 17:** Scatter plot for the water-quality parameter involving "Dissolved Oxygen" (2019)

![Temperature 2020](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/twentytemp.png)

**Figure 18:** Scatter plot for the water-quality parameter involving "Temperature" (2020)

![Conductance 2020](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/twentycond.png)

**Figure 19:** Scatter plot for the water-quality parameter involving "Specific Conductance" (2020)

![pH 2020](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/twentyph.png)

**Figure 20:** Scatter plot for the water-quality parameter involving "pH" (2020)

![Dissolved Oxygen 2020](https://github.com/cybertraining-dsc/fa20-523-312/raw/main/project/images/twentydox.png)

**Figure 21:** Scatter plot for the water-quality parameter involving "Dissolved Oxygen" (2020)


### 5.2 Centroid Calculation

The initial and final centroid values for the safe and unsafe water-quality standards are shown below for the year 2019. The predicted classes for the safe and unsafe clusters has also been shown below that directly follows from the previous results.

'''
Final centroid mu_safe:
Temperature          9.350000
Sp. Conductance    613.726744
pH                   8.424225
Dissolved O2        11.826163
dtype: float64

Final centroid mu_unsafe:
Temperature         10.672426
Sp. Conductance    658.729167
pH                   8.324755
Dissolved O2        10.910662
dtype: float64

Final cluster assignment:

      Temperature  Sp. Conductance   pH  Dissolved O2  Predicted_Class
0            10.2              559  8.4          10.2                0
1            10.1              559  8.4          10.2                0
2            10.1              560  8.4          10.2                0
3            10.0              560  8.4          10.3                0
4            10.0              561  8.4          10.2                0
...           ...              ...  ...           ...              ...
1327          7.6              670  8.3          10.7                1
1328          7.6              671  8.3          10.6                1
1329          7.6              671  8.3          10.6                1
1330          7.6              671  8.3          10.6                1
1331          7.6              671  8.3          10.6                1

'''

### 5.3 Heatmaps for the years - 2017, 2018, 2019, and 2020

For the all the four years, heatmaps were plotted to get more information about the trend of the data. Chiefly, the heatmaps give us an empirical form of ideology relating to the degree of correlation between the different water-quality parameters.

### 5.4 Analysis of sample set of values

In this portion, we test the unsupervised learning mechanism on the basis of sample set of water-quality values. In this regard, we feed the sample values to the coding framework and based on the centroids calculated for the past four years, it is able to identify whether the given water sample belong in the safe or unsafe category. Further, if it belongs in the unsafe category, the system can further inform us the degree of criticality of the water-quality degradation. This is carried out by finding out how many water quality parametric values are beyond the normal range. Based on this analysis, a critical nature is then displayed as shown in the figure below. As an example, a critical category of "2" would signify two of the water-quality parameters were beyond the normal range of values. Needless to say, higher is the critical category level, the more degraded the water source is.

### 5.5 Benchmark information

Finally, the benchmark analysis results are shown below for the respective tasks carried out by the coding platform. Two important facts should be kept in mind in this case and they are as follows:
- The benchmark analysis was carried out using the cloudmesh benchmark procedure in Python (executed in Google Colab). A sleep-time of "5" was selected as the standard for the benchmark analysis and it has followed consistently for all the calculations.
- The time values for the different benchmark results was not rounded off in this case as it was both important and interesting to know the minute differences between the different kinds of tasks that were carried out in this regard. It should be noted that the final benchmark value is exceptionally high since this step involves the part where the user inputs the sample values for ascertaining the safety standard for a water source.

'''
+------------------------------------------+----------+--------+--------+---------------------+-------+--------------+--------+-------+-------------------------------------+
| Name                                     | Status   |   Time |    Sum | Start               | tag   | Node         | User   | OS    | Version                             |
|------------------------------------------+----------+--------+--------+---------------------+-------+--------------+--------+-------+-------------------------------------|
| <ipython-input-6-76432cd55eb5>/<module>  | ok       |  9.929 |  9.929 | 2020-12-07 11:03:29 |       | a3eaca400b9c | collab | Linux | #1 SMP Thu Jul 23 08:00:38 PDT 2020 |
| <ipython-input-8-369a8f571c92>/<module>  | ok       |  5.275 |  5.275 | 2020-12-07 11:03:48 |       | a3eaca400b9c | collab | Linux | #1 SMP Thu Jul 23 08:00:38 PDT 2020 |
| <ipython-input-10-c44a9c976e98>/<module> | ok       |  5.477 |  5.477 | 2020-12-07 11:04:07 |       | a3eaca400b9c | collab | Linux | #1 SMP Thu Jul 23 08:00:38 PDT 2020 |
| <ipython-input-12-ce973ed94129>/<module> | ok       |  5.091 |  5.091 | 2020-12-07 11:04:24 |       | a3eaca400b9c | collab | Linux | #1 SMP Thu Jul 23 08:00:38 PDT 2020 |
| <ipython-input-14-7f046bc96145>/<module> | ok       | 80.721 | 80.721 | 2020-12-07 11:04:48 |       | a3eaca400b9c | collab | Linux | #1 SMP Thu Jul 23 08:00:38 PDT 2020 |
+------------------------------------------+----------+--------+--------+---------------------+-------+--------------+--------+-------+-------------------------------------+
'''

## 6. Conclusion

Although the endeavor carried out in this example might not involve a plethora of high-end applications or intricate logic frameworks, it still provides a very decent foundational approach for carrying out toxicological analysis for water sources. Most importantly, it should be noted that the results obtained for sample values correspond to what we would normally expect for polluted and non-polluted sources of water. For instance, it was found that water sources with high values of specific conductance were categorized in the "unsafe" category which is to be expected since a high conductance value typically represents the presence of dissolved salts and ions in the water source, which normally indicates that effluents or agricultural run-off might have made its way to the water source. Additionally, it was also found out that water samples with high values of dissolved oxygen levels were categorized in the "safe" category which is certainly true.

Of course, a more diverse array of data coupled with more scientific and advanced ASV systems would have provided us with even better results. But as indicated earlier, this research endeavor provides a pragmatic foundational approach to conducting this kind of big data analytical work. We can build up on the logic presented in this endeavor to come up with even more advanced and robust version of toxicological analysis.


## 7. Acknowledgements

The author would like to thank Dr. Gregor von Laszewski, Dr. Geoffrey Fox, and the associate instructors in the *FA20-BL-ENGR-E534-11530: Big Data Applications* course (offered in the Fall 2020 semester at Indiana University, Bloomington) for their continued assistance and suggestions with regard to exploring this idea and also for their aid with preparing the various drafts of this article.

## 8. References

[^1]: Valada A., Velagapudi P., Kannan B., Tomaszewski C., Kantor G., Scerri P. (2014) Development of a Low Cost Multi-Robot Autonomous Marine Surface Platform. In: Yoshida K., Tadokoro S. (eds) Field and Service Robotics. Springer Tracts in Advanced Robotics, vol 92. Springer, Berlin, Heidelberg. <https://doi.org/10.1007/978-3-642-40686-7_43>

[^2]: M. Ludvigsen, J. Berge, M. Geoffroy, J. H. Cohen, P. R. De La Torre, S. M. Nornes, H. Singh, A. J. Sørensen, M. Daase, G. Johnsen, Use of an Autonomous Surface Vehicle reveals small-scale diel vertical migrations of zooplankton and susceptibility to light pollution under low solar irradiance. Sci. Adv. 4, eaap9887 (2018). <https://advances.sciencemag.org/content/4/1/eaap9887/tab-pdf>

[^3]: Verfuss U., et al., (2019, March). A review of unmanned vehicles for the detection and monitoring of marine fauna. Marine Pollution Bulletin, Volume 140, Pages 17-29. Retrieved from <https://doi.org/10.1016/j.marpolbul.2019.01.009>

[^4]: USGS Water Quality Data, Accessed: Nov. 2020, <https://waterdata.usgs.gov/nwis/qw>

[^5]: EPA Water Quality Data, Accessed Nov. 2020, <https://www.epa.gov/waterdata/water-quality-data-download>

[^6]: Read, E. K., Carr, L., De Cicco, L., Dugan, H. A., Hanson, P. C., Hart, J. A., Kreft, J., Read, J. S., and Winslow, L. A. (2017), Water quality data for national‐scale aquatic research: The Water Quality Portal, Water Resour. Res., 53, 1735– 1745, doi:10.1002/2016WR019993. <https://agupubs.onlinelibrary.wiley.com/doi/epdf/10.1002/2016WR019993>

[^7]: Atlas Scientific team. *Atlas Scientific Environmental Robotics*. Retrieved from <https://atlas-scientific.com/>

[^8]: Sinha, Saptarshi. (2020) *A Big-data analysis framework for Toxicological Study*. Retrieved from <https://github.com/cybertraining-dsc/fa20-523-312/blob/main/project/code/toxicologyASV.ipynb>

[^9]: Google Colaboratory team. *Google Colaboratory*. Retrieved from <https://colab.research.google.com/>

[^10]: Tan, Steinback, Kumar (2004, April). Introduction to Data Mining, Lecture Notes for Chapter 8, Page 2. Accessed: Nov. 2020, <https://www-users.cs.umn.edu/~kumar001/dmbook/dmslides/chap8_basic_cluster_analysis.pdf>

[^11]: Alan J. (2019, November). K-means: A Complete Introduction. Retrieved from <https://towardsdatascience.com/k-means-a-complete-introduction-1702af9cd8c>
