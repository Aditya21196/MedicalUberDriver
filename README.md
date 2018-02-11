# TEAM NAME – CODING SENSEI

Alternate app for users- https://github.com/ajaylather/MedicalUberUser

## PRODUCT NAME- MEDICAL UBER

### Summary

The reach of technological innovation continues to grow, changing all industries as it evolves. In Healthcare, technology is increasingly playing the role in almost all processes, from patient registration, data monitoring , from lab tests to Self – Care tools. Devices like Smartphones and Tablets are starting to replace conventional monitoring and recording Systems and people are now giving the option of undergoing a full consultation in the privacy of their own homes. Technological advancements in Healthcare have contributed to services , being taken out of the confines of hospital walls and integrating them with user friendly devices.
Despite all this technological advancement, timely medical care at crucial times like at highways or at unknown places is very difficult to get. In our effort to solve this problem to some extent, we propose a the solution – Medical Uber , which takes the location of user and points out the nearest Hospital and ambulances at his convenience. It also informs the ambulance driver of the whereabouts of the patient.

#### Background
A Report on Road Accidents in India 2016, published by Transport Research wing under Ministry Of Road Transport and Highways, Government Of India, has revealed that more people died on roads accidents in India last year as compared to number of Deaths in 2015. So, Timely medical care is extremely Important.

##### Goals
1) To Reduce the time taken by the ambulance to reach the victims.
2) To reduce the latency of deliverance of medical help.
3) To potentially save lives. 
4) To Uberise ambulances.
5) To learn how to collaborate with a team (Personal Objective).
6) To incentivise ambulance drivers to pick up patients in need.

### Technologies Used 

Languages Used – XML, JAVA 
IDE Used – Android Studio
API's Used – Geolocation, Maps, 
Cloud Service – Google Firebase
Data Mining – Python was used for gathering data points.


### Features of the App

The app is made in 2 parts - one is for users and one is for ambullance drivers. When an ambulance driver logs in, a function is called which records the location of the driver and sends it to the user after every 10 seconds. He object transmitted to the server also records the UID of the driver. On the other hand, the client side app accesses the database and the notes the coordinates of the ambulances and shows them on a map. An OnClick listener is added to every marker. On clicking the marker, the contact details and co-ordinates of the user are sent to the driver associated to the UID of the marker. The driver then may navigate to the user while constantly tracking him. 


Following shows the logic behind our backend. It shows how we were intending to handle the incoming location updates on firebase:

![Alt text]( https://raw.githubusercontent.com/ajaylather/h4n/master/firebase%20code.png  "Child event listener for the user's app")

Following shows our code for starting Location Updates:

![Alt text](https://raw.githubusercontent.com/ajaylather/h4n/master/ss.png  "Location Update")


The following three images display the lifecycle of a location entry on our backend:

![Alt text](https://raw.githubusercontent.com/ajaylather/h4n/master/ss1.png  "Optional title")
![Alt text](https://raw.githubusercontent.com/ajaylather/h4n/master/ss2.png  "Optional title")
![Alt text](https://raw.githubusercontent.com/ajaylather/h4n/master/ss3.png  "Optional title")



### Extensions
While making the project, we came across many ideas to scale the app in terms of functionality and database as well as scope to improve upon the existing capabilities and design. Some of them are:

1) We understand that we only need to display the drivers nearby whereas our app displays all the ambulance drivers online. Geolocation API may be used to accompolish the same.

2)  We could also include the hospitals and contact numbers of those respective hospitals as part of our static database (along with their location).

3) While the ambulance in enroute to the user, an audio interface can be opened to interact with the patient and people nearby so that the nurse can give advice on how to provide temporary relief to the user.

4) Another static database can be used which can be leveraged to filter out the location and phone number of nearest hopital in the vicinity. It is possible to implement this feature in offline mode is the database will be static and only user location would be required which can simply be obtained from the GPS(assuming that the GPS signals are sufficiently strong).

### Shortcomings
1) Because of our lack of prior knowledge of the APIs, we were unable to leverage the API's to full effect. Data mining thus took too long we were exhausted even before we started with the development phase.

2) In hilly areas, there will be spurious signals because of which the app may not function as well as required.

3) Our idea is logically sound but we haven't yet delivered the full product. Though our team intends to work upon it in near future.
