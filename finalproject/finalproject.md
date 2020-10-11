# <ins>Aquatic Toxicity Analysis with the aid of Autonomous Surface Vehicle (ASV)</ins>

* [ ] remove all ins, nd /ins as it  will impact uniform formatting. E.g. we do not do wysiwyg we do markdown. ins is not markdown
* [ ] sections do not have colons at the end
* [ ] you do not have a refernce section.
* [ ] please rename the directory to "project", please rename the report to report.md. 
* [ ] all http links that are not res, must be in smaller, greater brackets.
* [+] this is a done item. Once you have done the item mar them with [+]


Saptarshi Sinha, fa20-523-312

## <ins>Research Statement:</ins>

When it comes to revolutionizing our qualities of life and improving standards, there is not another branch of science and technology that has made more impact than the myriad technological capabilities offered by the areas of Artificial Intelligence (AI) and its sub-fields involving Computer Vision, Robotics, Machine Learning, Deep Learning, Reinforcement Learning, etc. It should be borne in mind that AI was developed to allow machines/computer processors to work in the same way as the human brain works and which could make intelligent decisions at every conscious level. It was meant to help with tasks for rendering scientific applications more smarter and efficient. There are many tasks that can be performed in a far more dexterous fashion by employing smart-machines and algorithms than by involving human beings. But even more importantly, AI has also been designed to perform tasks that cannot be successfully completed by employing human beings. This could either be due to the prolonged boredom of the task itself, or a task that involves hazardous environments that cannot sustain life-forms for a long time. Some examples in this regard would involve exploring deep mines or volcanic trenches for mineral deposits, exploring the vast expanse of the universe and heavenly bodies, etc. And this is where the concept employing AI/Robotics based technology fits in perfectly for aquatic monitoring and oceanographical surveillance based applications.
 
Toxicity analysis of ecologically vulnerable water-bodies, or any other marine ecosystem for that matter, could give us a treasure trove of information regarding biodiversity, mineral deposits, unknown biophysical phenomenon, but most importantly, it could also provide meaningful and scientific information related to the biodegradation of the ecosystem itself. In this research project, an attempt will be made to design a simple foundation of an aquatic Autonomous Surface Vehicle (ASV) that will be deployed in marine ecosystems. Such a vehicle would be embedded with different kind of electronic sensors, that are capable of measuring physical quantities such as temperature, pH, conductance, dissolved oxygen level, etc. The data collected by such a system can either be over a period of time (temporal data), or it could cover a vast aquatic geographical region (spatial data). This data will then be compared with existing datasets that are made publicly available by various environmental organizations in the United States, most importantly the Environmental Protection Agency (EPA) and the US Geological Survey (USGS). A comparative data analysis task between the data collected by the ASV and the vast array of environmental data that are made available from these agencies can then give us an indication about the status of the aquatic degradation of the ecosystem in question by measuring the extent to which the current data deviates from relevant historical data trends. 


## <ins>Background Research and Previous Work:</ins>

After reviewing the necessary background literture and previous work that has been done in this field, it can be stated that most of such endeavors focussed majorly on continuous environmental data collection with the help of sensors attached to a stationary buoy in a particular location of a water-body. Some of the other endeavors did involve deploying a non-stationary vehicle that collected data from large swaths of geographical areas in a particular water body. However, neither did such attempts focus much on the data analysis portion for multiple sensory input(s) nor did it involve an intricate procedure to compare the collected data with historical trends so as to arrive at a suitable conclusion regarding the extent of environmental degradation.

As mentioned in the previous section, this research project will exhaustively focus not just on the data-collection portion by a non-stationary vehicle, but it will also involve employing deeper study towards the subject of big-data analysis of both the current data of the system in question and the past data obtained for similar aquatic profiles. In this way, it would be possible to learn more about the toxicological aspects of the ecosystem in question.



## <ins>Choice of data-set(s):</ins>

Upon exploring a wide array of available datasets, the following data repositories were chosen to get the required water quality based data over a particular period of time and for a particular geographical region.   

1. USGS Water Quality Data: https://waterdata.usgs.gov/nwis/qw
2. EPA Water Quality Data: https://www.epa.gov/waterdata/water-quality-data-download

To answer the questions involving existence of multiple data-sets and motivation of using multiple data-sets, we must keep in mind that the very nature of this study is based on historical trends of the how the water-quality has altered in the past and how it relates to the current situation. Because of these reasons, multiple data-sets will be referred to from multiple sources so as to achieve a robust data-analytical results. This would ensure that too much focus is not given on outlier cases, that may be relevant to just a particular geographical region or an aberration in the data that may only have arisen due to an unknown underlying phenomenon or some form of cataclysmic event from the past. Using multiple datasets from different sources would help to get a resultant data structure that is more likely to converge towards an approximate level of historical thresholds and which can then be used to find out how the current observed data deviates from such previous patterns.
   

## <ins>Proposed Methodology:</ins>

### Hardware Component:

A very rough outline of the autonomous surface vehicle (ASV) in question has been preceived in the Autodesk Fusion 360 software model. A preliminary model has been erected in this software so as to 3D print the design and then interface it with the appropriate sensors in question. Then system will be driven by an Arduino-Uno based microcontroller, and it will have different types of environmental sensors that will collect and log data. These sensors have been purchased from the vendor, "Atlas Scientific". As of now, the sensors that have been chosen for this ASV are as follows: 

* PT-1000 Temperature sensor kit - https://atlas-scientific.com/kits/pt-1000-temperature-kit/
* Potential of Hydrogen (pH) sensor kit - https://atlas-scientific.com/kits/ph-kit/
* Dissolved Oxygen (DO) sensor kit - https://atlas-scientific.com/kits/dissolved-oxygen-kit/
* Conductivity K 1.0 sensor kit - https://atlas-scientific.com/kits/conductivity-k-1-0-kit/

### Software Component:

After the data has been collected by the ASV either on a temporal scale (over a period of time) or a spatial scale (over a geographical area), it will then be analyzed to decipher the median convergent values of the water body for the four different parameters that have been measured (i.e. Temperature, pH, DO, and Conductivity). The results of this data analysis task will then be used to find out if such water quality parametric values manifested by the aquatic ecosystem in question deviates by a large proportion from the other result that is obtained after analyzing the historical data from USGS and EPA for a nearby and unpolluted source of water. The USGS and EPA websites make it easier to find data from a nearby geographical region by making it possible to enter the desired location prior to searching for water quality data in their huge databases. In this way, it can be figured out if the water quality parameters of the particular ecological system varies wildly from a neighboring system that has almost the same geographical and ecological attributes.

The establishment of the degree of variance of the data from the historical data will be carried out by documenting the particular quartile range that the current data lies in with respect to the median data that is obtained from the past/historical datasets. For instance, if the current data resides in the second quartile, it can be demarcated as being more or less consistent with previously established values. However, if it resides in the first or third quartile then it might will that the system has aberrant aspects which might need to be investigated for possible levels of outside pollutants (viz. industrial effluents, agricultural wash-off, etc.), or presence of harmful invasive species that might be altering the delicate natural balance of the ecosystem in question.


## <ins>Inference:</ins>

This section will be addressed upon project completion.

## <ins>Conclusion and Future Direction(s):</ins>

This section will be addressed upon project completion.
