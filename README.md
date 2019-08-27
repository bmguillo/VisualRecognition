# Provision Watson Visual Recognition Service & Create a customer image classifier for training


Step 1: Provision Instance of Visual Recognition
- In order to have seperate instances for QA, Staging, Dev & Prod
- Provision Standard instances
- Lite instances are not suitable for production

![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic1.png)
![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic2.png)

Step 2: Create a Custom Model
- Click on Manage to reach main landing page for Visual Recognition where credentials are found

![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic3.png)



Step 3: Create a custom Visual Recognition classifier
- We need a custom classifier because the images we are training on go beyond the built-in image classifiers since they go beyond objects, faces and food

![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic4.png)






Additional Resources:
- [Getting Started Documentation](https://cloud.ibm.com/services/watson-vision-combined/crn%3Av1%3Abluemix%3Apublic%3Awatson-vision-combined%3Aus-south%3Aa%2F7d079bae5542b868586749125bad3e5b%3A719b0d28-22c9-489c-ae7b-2bfab84a857b%3A%3A?paneId=gettingStarted&new=true)
- [Visual Recognition API documentation](https://cloud.ibm.com/apidocs/visual-recognition)



