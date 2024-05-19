# SE101 Design Project - Autonomous Tank for Food Delivery

Team Members: Elijah Kurien, Alice Zhao, Ian Korovinsky, Krish Modi, Patrick Huang, Rajan Agarwal

SE 101 Repository

Our self-driving car project aimed to develop an autonomous delivery vehicle for the University of Waterloo campus. We used OpenCV for tasks like pathfinding and lane detection on walking paths. By converting Google Maps satellite images into black-and-white pixels and applying color thresholds, we isolated walking paths and assigned coordinates to create precise maps. This enabled accurate navigation between any two points on campus.

We then mounted a camera on the vehicle to distinguish between grass and walking paths. Using image processing techniques such as composite masking and edge detection, we extracted distances and identified obstacles. This data fed into a neural network that made real-time navigation decisions. Despite challenges like variable path widths and shadows, our approach allowed the vehicle to navigate accurately.

Due to computational limits, we used a Raspberry Pi for initial data processing and offloaded intensive tasks to an external server. The server analyzed live video and sensor data, sending motor instructions back to the vehicle. Error control mechanisms, including PCB encoders, improved GPS accuracy and tracked the vehicle's movement precisely. OpenCV was crucial for mapping, real-time path extraction, and robust error management, enabling successful autonomous navigation.
