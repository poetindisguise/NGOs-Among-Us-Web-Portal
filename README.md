# NGOs-Among-Us-Web-Portal
* As a component of the Software Engineering course, we have built a web application where NGOs, Donors and Volunteers can register and carry out various operations.
* Used NodeJS and Express for backend, React for frontend and MongoDB Atlas as the database.
* Agile methodologies of SCRUM were followed.
* Youtube link of demo: https://youtu.be/t8YcBV_AmGk
* Heroku link: https://ngoamongus.herokuapp.com/
## Project Overview
Often, philanthropists desire to donate money, clothes, books etc. to NGOs in their city whom they can trust. Some people even want to volunteer to help the underprivileged for the well being of the society. However, due to lack of awareness, donors might not know about the existence and details of NGOs located near them. Also, many a time it is difficult for a person to contact somebody and ask whether any activity is going on at their organization for which they can volunteer. There is no central system wherein all the details of NGOs could be provided. <p>
Hence, we present to you our web portal <b>“NGOs Among Us”</b>, which makes an effort to bridge the gap between users and NGOs. The portal will provide the user with an option to register as a donor as well as volunteer. Furthermore, an NGO can enter its details and sign up with our portal. They can add documents and images of their welfare activities. The server helps the user by displaying a list of registered NGOs situated near him/her. <p>
The Volunteers will be able to know the schedule of the NGOs' social work so that they can collaborate with the Organization. All the work done by the NGO can be seen by the donors registered who can either donate money or essentials if they find the NGO trustworthy. Users may also rate the NGO based on their experience. Overall, the Portal will help both the people who want to donate as well as the NGOs who want to serve the society. <p> 
  
## Use case diagram
<img src="https://user-images.githubusercontent.com/66271769/127736217-ebb18a71-7353-4250-9a05-ff8718d61644.PNG" width="550" height="400">

## Class diagram
<img src="https://user-images.githubusercontent.com/66271769/127736279-66095267-7a7a-45e0-9202-967c8a9b7269.PNG" width="500" height="350">

 ## Sample Screenshots
  ### Homepage
  
 <img src="https://user-images.githubusercontent.com/66271769/127736787-406f51f1-41a7-4510-bb54-b74f17696f80.PNG" width="600" height="350">
  
  ### Volunteering schedule of NGO
  
 <img src="https://user-images.githubusercontent.com/66271769/127736790-731ea4c0-19eb-4144-a696-da66488b7b93.PNG" width="550" height="600">
  
  ### User profile
  
 <img src="https://user-images.githubusercontent.com/66271769/127736792-c7c8840a-9520-42ec-8c73-d23c3ef5b813.PNG" width="550" height="300">
 
 <img src="https://user-images.githubusercontent.com/66271769/127736793-6d9e143d-8d10-4252-af3a-61e2ea10c2d9.PNG" width="550" height="300">
  
  ### Donation
  
 <img src="https://user-images.githubusercontent.com/66271769/127736794-8e08e8e6-7287-4e76-b9f9-655a8244e1cb.PNG" width="550" height="350">
 <img src="https://user-images.githubusercontent.com/66271769/127736796-d61f3afc-c8d0-41b7-9f49-2a59107ae310.PNG" width="550" height="350">
  
  ### View Donations
  
 <img src="https://user-images.githubusercontent.com/66271769/127736797-02bc3ea4-68a9-4d36-8a6b-d2b3a1583e1d.PNG" width="550" height="300">
  
## NoSQL documents
  
  <img src="https://user-images.githubusercontent.com/66271769/127737646-5daa8486-7dac-4e04-9aab-270653ee30df.PNG" width="550" height="600">

* Referencing is done in “Ngos” collection to “Categories” collection via categoryID when a new NGO is being added.
* Referencing is done in the “Donations” collection to “Users” collection via donorID when a new donation is made.
* Referencing has also been done in “Donations” collection to “Ngos” collection via receiverID when a new donation is received by an ngo.
* Embedding is not used in our database system. 
* Denormalization is absent in the database system because we are not storing any duplicate field names. Thus our data would be consistent across various collections.
  
## Summary of the problem and work done :

The aim of the project was to build a portal which will connect NGOs to people. People who want to donate and work with NGOs have a hard time finding the right NGO. This problem exists on the other side as well because it is hard for NGOs with limited funding to reach out to people and inform them about their organization. This very problem is solved by our portal which lists all the NGOs around the people. We had started off by building basic features like listing the details of the NGOs. Search and Sort functionality were added based on the name, rating and category of the NGO. The Volunteer would require the work schedule of the NGO so the portal asks the NGO for it which can be updated later on. Features like rating, monetary donation and essential item donations were added, later part of which gets stored and can be viewed by both NGOs and donors.

## Future scope
  We suggest the <b>MICROSERVICE ARCHITECTURE for our future scaled-up system.</b>
  <img src="https://user-images.githubusercontent.com/66271769/127737805-a77a5ce9-ac4e-4b4c-9058-7a037967ee28.PNG" width="600" height="600">


