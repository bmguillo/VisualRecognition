# Provision Watson Visual Recognition Service & Create a customer image classifier for training


Step 1: Provision Instance of Visual Recognition
- Choose region and resource group
- In order to have seperate instances for QA, Staging, Dev & Prod, provision Standard instances
- Lite instances are not suitable for production

![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic1.png)
![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic2.png)

Step 2: Create a Custom Model
- Click on Manage to reach main landing page for Visual Recognition where credentials are found

![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic3.png)



Step 3: Create a custom Visual Recognition classifier
- We need a custom classifier because the images we are training on go beyond the built-in image classifiers since they go beyond objects, faces and food
- Click on classify images/create model tile

![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic4.png)

Step 4: Create a project for your custom model and add Watson Visual Recognition service
- Provide a name, description
- This project automatically integrates Cloud object storage for storage of the images, provisions automatically
- Uncheck restrict collaborators if no confidential data, not using SAML for authentication & only IBM Cloud account users accessing the project
- Click add to add Visual recognition service
- Choose existing, choose resource group and service we provisioned prior

![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic5.png)

Step 5:



Additional Resources:
- [Getting Started Documentation](https://cloud.ibm.com/services/watson-vision-combined/crn%3Av1%3Abluemix%3Apublic%3Awatson-vision-combined%3Aus-south%3Aa%2F7d079bae5542b868586749125bad3e5b%3A719b0d28-22c9-489c-ae7b-2bfab84a857b%3A%3A?paneId=gettingStarted&new=true)
- [Visual Recognition API documentation](https://cloud.ibm.com/apidocs/visual-recognition)



