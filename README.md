Application Programming Interfaces (APIs) defines interactions between multiple intermediaries. In this case, APIs allow for the collection of data from third party software services such as OpenWeather and GoogleMaps to produce datasets
for analysi and maps for visualization of data. The two examples in this repository demonstrate these functionalities. WeatherPy demonstrates the retrieval of data through APIs; while VacationPy demonstrates the utility of the Google Maps API in
visualizing that data. 

WeatherPy: Using online weather data. 
This project involves two parts: Part One is the generation of data for analysis; and Part Two is the analysis of the generated data through a series of linear regressions using Pandas.
I have demondtrated the utility of these two tools before  for the handling and analysis of vast amounts of data; and for the creation of visual representations of that data. These analyses revolve around four main avenues of inquiry concerning  global climatic trends i relative to latitude: 

Latitude versus Temperature
It is more or less common knowledge that climate tends to trend on the hotter side as one moves closer to the lower latitudes closer to the equator. This regression tests that notion and suggests it to be generally true.
 The relationship between the two is robust in both Northern (r= -0.877), and Southern (r= 0.546) hemispheres. Plot 1.1 demonstatrates the U-shaped trend as higher temperatures are recorded  around the Equator then consistently decline as one moves further toward the Poles. This trend is elaborated upon by Plots 2.1 and 3.1. 
Equations 1.1 and 2.1 express these trends in mathematical terms. 

Latitude versus Humidity
Plot 1.2 shows that humidity tends to fall, on average, on the higher end globally. In Plot 2.2, the Northern Hemisphere shows a trend toward higher humidity, on average as ne appraches the Arctic; but this trend is largely due to the greatly reduced variability as fewer low humidity readings are recorded. 
Plot 3.2 shows a trend toward rising humidity in the Southern Hemisphere as one approaches the Equator. This paradoxical incongruity in hemispheric trends does not have a theoretical explanation although both seem to be due to a decline in variability in the latitudes in question. 

Latitude versus Cloudiness
Plot 1.2 shows that cloudiness is an apparently random phenomenonacross the globe. Cloudiness does not appear to follow a consistent trend  with latitude in the Northern Hemisphere (r=0.0.257), or the Southern Hemisphere (r=-0.081). What is apparent is that there are clusters of data points that appear to cluster around clear skies and heavy cloud cover. These clusters appear to be wholly independent of latitude
This is apparrent in Plot 1.3, where  the vast majority of data points appear to fall on the extreme ends of clear skies (0%) and complete overcast (100%).  There are large numbers of data points in between. that don't seem to form patterns that meaningfully coincide with latitude. Overall, cloudiness is a highly variable phenomenon that may change quickly depending on the time an observation is recorded; and that may also contribute to the noisiness of this data. 


Latitude versus Wind Speed
Wind speed is pretty straightforward. It is expected to be highly variable and to vary wildly depending on when it was recorded. Plot 1.4 sypports this supposition; and it shows that wind speeds typically don't go above 10 mph.Wind Speed has a limited relationship with Latitude. 
There are noticeable spikes in the middle latitudes of both Hemispheres (Plots 2.4 & 3.4); but this relationship is not really predictive in either the Northern (r= -0.245), or Southern Hemisphere (r= -0219)
It would be helpful to note that Big Data, while greatly illuminaing, is not perfect.The existence of a mathematical relationship between two vatiables does not PROVE a causal relationship between them. Data can show  that temperature increases as one moves into lower latitudes; but data cannot explain why without proper context and interpretation. 
Practitioners of research design are familiar with the term "validity" to describe how good research design has to ensure that quantification properly measures whatever phemomenon it claims to measure. 

VacationPy: 

This mini-project makes use of the data from WeatherPy and integrates it with a GoogleMaps interface tp generate an overlay of potential vacation destinations with weather data. Aside from showing mathematical relationships, data is also useful in guiding human decision-making, This kind of information display can be helpful for prospective vacationers in planning and making their travel arangements. 
As with making conclusions from data,  this exercise demonastrate not just the utility of huge amounts of data; but the importance of good visualization in making large amounts of data comprehensible to the average person. For example, the Humidity Heatmap vondenses data from more than 600 places globally and condenses it into an intuitively understandable image. The hotelmap is ano example of how multiple APIs can work together to collect and visualize data.
