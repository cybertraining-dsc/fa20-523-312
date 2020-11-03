# Aquatic Toxicity Analysis with the aid of Autonomous Surface Vehicle (ASV)

Saptarshi Sinha, [fa20-523-312](https://github.com/cybertraining-dsc/fa20-523-312/), [Edit](https://github.com/cybertraining-dsc/fa20-523-312/blob/master/project/project.md)

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

After reviewing the necessary background literture and previous work that has been done in this field, it can be stated that most of such endeavors focussed majorly on continuous environmental data collection with the help of sensors attached to a stationary buoy in a particular location of a water-body. Some of the other endeavors did involve deploying a non-stationary vehicle that collected data from large swaths of geographical areas in various water bodies [^1]. Other research attempts focussed on niche areas such as study of the migration pattern exhibited by zooplanktons upon natural and aritifical irradiance [^2], and detection and monitoring of marine fauna [^4]. However, neither did such attempts focus much on the data analysis portion for multiple sensory input(s) nor did it involve an intricate procedure to compare the collected data with historical trends so as to arrive at a suitable conclusion regarding the extent of environmental degradation.

As mentioned in the previous section, this research project will exhaustively focus not just on the data-collection portion by a non-stationary vehicle, but it will also involve employing deeper study towards the subject of big-data analysis of both the current data of the system in question and the past data obtained for similar aquatic profiles. In this way, it would be possible to learn more about the toxicological aspects of the ecosystem in question.


## 3. Choice of Data-sets

Upon exploring a wide array of available datasets, the following data repositories were chosen to get the required water quality based data over a particular period of time and for a particular geographical region.   

1. USGS Water Quality Data: <https://waterdata.usgs.gov/nwis/qw>
2. EPA Water Quality Data: <https://www.epa.gov/waterdata/water-quality-data-download>

The USGS dataset is very commensurate with the research goal of this endeavor and hence, focus will be put more on the USGS dataset over the EPA dataset. Some previous work was conducted on this USGS dataset by a particular research team [^3]. However, the emphasis of such work was done from a very broad perspective so as to create an overview of how to use and visualize the data from the USGS water quality portal. Besides, such a work emphasizes on characterizing the seasonal variation of lake water clarity in different regions throughout the continental US, something that is very deviant from what would be addressed in this particular article which majorly involves environmental degradation and toxicology analysis using an autonomous surface vehicle.  

To address the questions involving existence of multiple data-sets and motivation of using multiple data-sets, we must keep in mind that the very nature of this study is based on historical trends of the nature of water-quality in a particular region from the past and how it relates to the current situation. Because of these reasons, multiple data-sets will be referred to from multiple sources so as to achieve robust data-analytical results. This would ensure that too much focus is not given on outlier cases, that may be relevant to just a particular geographical region or an aberration in the data that may only have arisen due to an unknown underlying phenomenon or some form of cataclysmic event from the past. Using multiple datasets from different sources would help to get a resultant data structure that is more likely to converge towards an approximate level of historical thresholds and which can then be used to find out how the current observed data deviates from such previous patterns.
   

## 4. Methodology

### 4.1 Hardware Component

The rough outline of the autonomous surface vehicle (ASV) in question has been perceived in the Autodesk Fusion 360 software model. A preliminary model has been designed in this software so as to 3D print the system. It will then be interfaced with the appropriate sensors in question. Then system will be driven by an Arduino-Uno based microcontroller, and it will have different types of environmental sensors that will collect and log data. These sensors have been purchased from the vendor, "Atlas Scientific". As of now, the sensors that have been chosen for this ASV are as follows: 

* PT-1000 Temperature sensor kit - <https://atlas-scientific.com/kits/pt-1000-temperature-kit/>
* Potential of Hydrogen (pH) sensor kit - <https://atlas-scientific.com/kits/ph-kit/>
* Dissolved Oxygen (DO) sensor kit - <https://atlas-scientific.com/kits/dissolved-oxygen-kit/>
* Conductivity K 1.0 sensor kit - <https://atlas-scientific.com/kits/conductivity-k-1-0-kit/>

A very rudimentary framework of the system has been realized in the Autodesk Fusion 360 software architecture as shown below. The design provided below is a very simplistic platform but which will lay the foundation of the final structure of the system (see Figure 1).

![ASV from Fusion 360](https://github.com/cybertraining-dsc/fa20-523-312/raw/master/project/images/ASVSS1.png)
     
**Figure 1:** Nascent framework of the ASV system in Fusion 360

With the chassis framework out of the way, a careful analysis was conducted towards the successful developmental work to be done to complete the build process for a fully functional prototype ASV. In essence, an ASV can be thought of being composed of certain key sub-elements. From a broad perspective, they comprise the hardware makeup, a suitable propulsion system, a sensing system, a communication system, and an appropriate source of onboard power source. The hardware makeup being out of the way, the other aspects can now be elaborated as follows:

**Propulsion System:** The two possibilities that was considered in this regard involve using either a single servo motor with an assortment of rudders and propellers for appropriate steering, or using two separate servo motors, one of which will drive the left-hand side of the system and the other would drive the right-hand side. The second arrangement is preferred in this regard as it provides with better maneuverability and control of the system. For instance, to move forward in a rectilinear fashion, both the motors would be given the same level of power. Whereas for steering the system in a particular direction, one of the motors would be assigned a lower power level than the other, thereby enabling the system to curve inwards on the side which has the motor with a lower power level. Of course, there will always be perturbations and natural disturbances that will deter the system from making these correct path changes. For this reason, a Proportional-Integral-Derivative (PID) controlled response would be augmented for the locomotion algorithm.

**Sensing System:** As discussed previously, an arrangement involving four different sensors will be integrated in the ASV. This way, when the entire ASV system is deployed in an aquatic environment, it will be able to simultaneously provide readings for all four water-quality parameters in this case. Precisely, these water-quality parameters would be temperature, potential of hydrogen (pH), dissolved oxygen level, and specific conductance value. It should be noted in this perspective that it is possible to include even more sensors in this ASV system. However, the reason why it was not necessary to go beyond these four sensor types is primarily because of two reasons. Firstly, these parameters are important to most toxicological analysis studies [^1] and the readings provided by such a sensory system could be considered as a foundation which could provide future directions (including adding more sensors, if needed). Secondly, we should also keep in mind that the hardware system has certain constraints. In this scenario, it involves a sensory shield (that can be integrated with the Arduino microcontroller) that is being used but which has a maximum of four ports for four different sensors only. Though it is possible to add another layer of shield on top of the current one (thereby raising the capability of integrating the number of sensors to eight), it adds unnecessary bandwidth issues, memory depletion possibilities, along with an increased demand of higher power supply. These issues will especially be more consequential in this case as we are dealing with a microcontroller that has limited memory and power, unlike a microprocessor. Hence, the decision to stick with four sensors only was made.

**Communication System:** This is possibly the most important part of the ASV system as we need to device a technique to offload the data that is collected by the vehicle back to a remote computer/server that would likely be located at a considerable distance away from the ASV. There are different options that have been considered in this regard for establishing a proper communicative functionality between the ASV and the remote computer. Some options that have been considered involved Bluetooth, IR signals, RF signals, GPS-based system, satellite communication, etc. There are both pros and cons when it comes to using any of these different communication systems for the ASV. However, the most important metric in this case involves the maximum range the communication system could span over. Obviously, some of the options (viz. Bluetooth) would not be possible in this regard as they have a very limited communication range. Some others (viz. satellite communication systems) have a very high range but were nevertheless found unsuitable for this endeavor as they required too much onboard processing power to even carry out their most basic operations. Hence, a balanced approach was followed in this scenario and a GPS/RF-based system was eventually chosen as the most appropriate candidate for carrying out the proposed tasks of the ASV.

**Power Source:** Finally, we need an onboard processing power system that can provide the required amount of power to all the functional entities housed in the ASV system. The characteristic of such a desired power source would be that it would not require charging often and can sustain proper ASV operations for at least five to six hours. Additionally, the weight of the power source should also not be too clumsy that might put the stability of the entire ASV system in jeopardy. It must have a suitable weight, and should also come in an appropriate shape and size such that the weight of the entire system is evenly distributed over a large area, thereby further reinforcing the stability of the system. 


### 4.2 Software Component

After the data has been collected by the ASV either on a temporal scale (over a period of time) or a spatial scale (over a geographical area), it will then be analyzed to decipher the median convergent values of the water body for the four different parameters that have been measured (i.e. Temperature, pH, DO, and Conductivity). The results of this data analysis task will then be used to find out if such water quality parametric values manifested by the aquatic ecosystem in question deviates by a large proportion from the other result that is obtained after analyzing the historical data from USGS and EPA for a nearby and unpolluted source of water. The USGS and EPA websites make it easier to find data from a nearby geographical region by making it possible to enter the desired location prior to searching for water quality data in their huge databases. In this way, it can be figured out if the water quality parameters of the particular ecological system varies wildly from a neighboring system that has almost the same geographical and ecological attributes.

The establishment of the degree of variance of the data from the historical data will be carried out by documenting the particular quartile range that the current data lies in with respect to the median data that is obtained from the past/historical datasets. For instance, if the current data resides in the second quartile, it can be demarcated as being more or less consistent with previously established values. However, if it resides in the first or third quartile then it might will that the system has aberrant aspects which might need to be investigated for possible levels of outside pollutants (viz. industrial effluents, agricultural wash-off, etc.), or presence of harmful invasive species that might be altering the delicate natural balance of the ecosystem in question.


## 5. Inference

NOTE: This section will continue to be updated until project completion.

The first preliminary set of results are displayed below. Here, the content of the dataset, after it is processed in a software architecture, is shown and it displays the alteration of the values (expressed in line plots, scatter plots, and histograms) of the four main water-quality parameters (viz. Temperature, Specific Conductance, pH, and Dissolved Oxygen) over the period of time that starts from October 9, 2020 to October 16, 2020.

![Temperature plots](https://github.com/cybertraining-dsc/fa20-523-312/raw/master/project/images/L_temp.png)
![Temperature plots](https://github.com/cybertraining-dsc/fa20-523-312/raw/master/project/images/S_temp.png)
![Temperature plots](https://github.com/cybertraining-dsc/fa20-523-312/raw/master/project/images/H_temp.png)
     
**Figure 2:** Line, Scatter, and Histogram plots for the water-quality parameter involving "Temperature"

![Specific Conductance plots](https://github.com/cybertraining-dsc/fa20-523-312/raw/master/project/images/L_cond.png)
![Specific Conductance plots](https://github.com/cybertraining-dsc/fa20-523-312/raw/master/project/images/S_cond.png)
![Specific Conductance plots](https://github.com/cybertraining-dsc/fa20-523-312/raw/master/project/images/H_cond.png)
     
**Figure 3:** Line, Scatter, and Histogram plots for the water-quality parameter involving "Specific Conductance"

![pH plots](https://github.com/cybertraining-dsc/fa20-523-312/raw/master/project/images/L_pH.png)
![pH plots](https://github.com/cybertraining-dsc/fa20-523-312/raw/master/project/images/S_pH.png)
![pH plots](https://github.com/cybertraining-dsc/fa20-523-312/raw/master/project/images/H_pH.png)
     
**Figure 4:** Line, Scatter, and Histogram plots for the water-quality parameter involving "pH"

![Dissolved Oxygen level](https://github.com/cybertraining-dsc/fa20-523-312/raw/master/project/images/L_dO2.png)
![Dissolved Oxygen level](https://github.com/cybertraining-dsc/fa20-523-312/raw/master/project/images/S_dO2.png)
![Dissolved Oxygen level](https://github.com/cybertraining-dsc/fa20-523-312/raw/master/project/images/H_dO2.png)
     
**Figure 5:** Line, Scatter, and Histogram plots for the water-quality parameter involving "Dissolved Oxygen level"

### First Benchmark results (Expected - November 11):

### Second Benchmark results (Expected - November 13):

### Third Benchmark results (Expected - November 15):


## 6. Conclusion

NOTE: This section will be addressed upon project completion.

## 7. Acknowledgements

The author would like to thank Dr. Gregor Von Laszewski, Dr. Geoffrey Fox, and the associate instructors in the *FA20-BL-ENGR-E534-11530: Big Data Applications* course (offered in the Fall 2020 semester at Indiana University, Bloomington) for their continued assistance and suggestions with regard to exploring this idea and also for their aid with preparing the various drafts of this article.

## 8. References

[^1]: Valada A., Velagapudi P., Kannan B., Tomaszewski C., Kantor G., Scerri P. (2014) Development of a Low Cost Multi-Robot Autonomous Marine Surface Platform. In: Yoshida K., Tadokoro S. (eds) Field and Service Robotics. Springer Tracts in Advanced Robotics, vol 92. Springer, Berlin, Heidelberg. <https://doi.org/10.1007/978-3-642-40686-7_43>

[^2]: M. Ludvigsen, J. Berge, M. Geoffroy, J. H. Cohen, P. R. De La Torre, S. M. Nornes, H. Singh, A. J. Sørensen, M. Daase, G. Johnsen, Use of an Autonomous Surface Vehicle reveals small-scale diel vertical migrations of zooplankton and susceptibility to light pollution under low solar irradiance. Sci. Adv. 4, eaap9887 (2018). <https://advances.sciencemag.org/content/4/1/eaap9887/tab-pdf>

[^3]: Read, E. K., Carr, L., De Cicco, L., Dugan, H. A., Hanson, P. C., Hart, J. A., Kreft, J., Read, J. S., and Winslow, L. A. (2017), Water quality data for national‐scale aquatic research: The Water Quality Portal, Water Resour. Res., 53, 1735– 1745, doi:10.1002/2016WR019993. <https://agupubs.onlinelibrary.wiley.com/doi/epdf/10.1002/2016WR019993>

[^4]: Verfuss U., et al., (2019, March). A review of unmanned vehicles for the detection and monitoring of marine fauna. Marine Pollution Bulletin, Volume 140, Pages 17-29. Retrieved from <https://doi.org/10.1016/j.marpolbul.2019.01.009>




