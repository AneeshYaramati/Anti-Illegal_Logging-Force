# Inspiration
We depend on forests for our survival, from the air we breathe to the wood we use. Besides providing habitats for animals and livelihoods for humans, forests also offer watershed protection, prevent soil erosion and mitigate climate change. Yet, despite our dependence on forests, we are still allowing them to disappear.

More than one in four people around the world relies on forest resources for their livelihoods.

Yet forests have effectively disappeared in 25 countries and another 29 countries have lost more than 90% of their forest cover.

Between 25% and 30% of the greenhouse gas released into the environment come from deforestation

Nearly two rangers a week are killed protecting the wildlife. Around 30,000 species are driven to extinction every year

90% of all wildfires are started by humans. Climate change, as predicted, is fueling longer, stronger, and quicker-to-start wildfires.

All the facts stated above are the inspiration for us the younger generation to come up with solution to stop the major factors degrading the forest ecosystem like illegal logging, poaching and forest fires with the help of emerging technologies including but not limited to IoT, Machine Learning and Blockchain.

# What it does
The main objectives of the proposed Forest Management System :

Prevention of illegal logging (Deforestation).
Forest Fire Detection.
Detection and Prevention of Animal Poaching.
Methodology
Sensor Nodes are placed across the forest.

# Where to place them ?

We use GIS ( Esri Arcgis ) to locate the entry, exit points, roads, pathway and any possible hotspots of the forest and place more sensors in that regions and comparatively less sensors in the deep forest.

How the sensors get their power supply in a forest ?

Solar Module for Arduino will be used that can power your Arduino/raspberry-pi board, to get a totally autonomous outdoor board. It includes a 3W solar panel that provides 5V to your Arduino/raspberry-pi board, and a 1100 mAh Li-Ion battery.

# What sensors are used ?

Sensors include flame, smoke detection sensors and temperature, humidity sensor to help us to detect forest forests.

Microphone, Camera module to capture voice, images of the surrounding which are inputs to the machine learning module which detects any suspicious sounds like chainsaw, heavy machinery, vehicles, gunshot, etc. and also detects humans(poachers, illegal loggers), vehicles, and other potential signs of poaching, logging from the captured images.

All the sensors are connected to arduino /raspberry pi based microcontroller, which gets it's power supply from solar module.

The sensor data is sent to the server with the help of esp8266 wi-fi microchip.

To provide internet access we can make use of starlink or similar technologies, with which we can have internet access with less hardware infrastructure (which is very essential in forest region) .

If any potential signs of threat observed, the details along with the location (with the help of GPS Module) will be sent to the forest rangers.

What if any node containing sensors gets destroyed due to forest fires or some other factors ?

In Such case, it is difficult to locate the source of the file as all the data present in that node would be destroyed, therefore we use IoT + Blockchain, In a blockchain each copy of data is kept at all nodes, if one gets destroyed it's data will still be available in the remaining nodes and therefore easy to find out the source.

# How we built it
List of the different types of sensors used :

Flame detection
Smoke detection
Temperature and humidity detection
GPS Module
Microphone
Camera Module
Solar Module for arduino
esp8266 wi-fi Module
All these embedded within a Arduino based microcontroller, which drives the power and collect the sensor data.

The sensor selection is based on several factors : Range, Power efficient, Cost efficient, weather resistant and several other factors .

We use esp8266 module to send sensor data to the server for further computation, run the ml-trained models.

Refer the flow-chart for the step by step procedure.

Machine Learning Model

We build a Machine learning based audio identifying model, with the help of ESC-10 dataset, a labeled set of 400 environmental recordings (10 classes, 40 clips per class). Attached a screenshot of a results achieved(Fig.3), where a chainsaw sound was given input the and model predicted the probability to which class(Fig.2) the sound belongs to.

Note : Numbering starts from 1 in Fig.2 and numbering starts from 0 in Fig.3 .

We are searching for image datasets to test, train model for object detection that recognized specific animals, as well as humans, vehicles, and other potential signs of poaching, logging.

# Business Opportunities
More then 100 MNC'S pledged to reduce their carbon footprint by 2030, we can work with these companies to offset their carbon footprint.

Since there are many natural lovers out there, we can launch an app/website which streams live sounds, videos from the forest.

From forest environment monitoring, we have large amounts of real-time data, we can put up that data for sale for analysis in the field of research and development.

We can also use IoT-based devices for real-time monitoring of animal health conditions and track the real-time location of the animal. And can provide data to local governments and organizations and work with them together.

# Challenges we ran into
Finding the audio dataset to test, train the model, shortlisting the sensors (to go with less number of sensors as possible because we have power consumption constraint). It's just the starting stage of the project (ideation stage) and hopefully we will clear all the obstacles and challenges that we face during the remaining process.

# What we learned
We learnt about blockchain technologies, Machine Learning, Working with various sensors and Arduino, Forest ecosystem, GIS.

# What's next for Forest Ecosystem Management
Include motor drivers, sprinkler for reducing forest fires, more advanced machine learning models to detect potential signs of poaching, logging, fires and also translate the trained model as an API.
