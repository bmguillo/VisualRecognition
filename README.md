# Provision Watson Visual Recognition Service & Create a customer image classifier for training via UI


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
- Choose existing, choose resource group and service we provisioned prior then click select
- Go back and refresh page to see Watson Visual Recognition populated
- Click create

![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic5.png)
![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic6.png)
![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic7.png)
![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic8.png)

Step 5: Name your Visual Recognition Model & Create a class(image classifier) to train positive images
- VR Model is the name of the Visual Recognition model in this example
- Genuine Image is the name of the class in this example
![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic9.png)

Step 6: Click in Genuine Image Image classifier and upload 10+ images to train the VR Model on positive images
- The more examples you provide the more the confidence increases
- Images must be uploaded to train as a zip file(for this example they are dogs stored in train folder called GenuineImages.zip)
- Upload by upload to project/add from project/add to model/drag & drop zip file options
![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic10.png)

Step 7: Use the built-in negative class to train the Watson Visual Recognition service on negative images
- The more examples you provide the more the confidence increases
- Images must be uploaded to train as a zip file(for this example they are images not dogs stored in train folder called NegativeImages.zip)
- Upload by upload to project/add from project/add to model/drag & drop zip file options
![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic11.png)

Step 8: Train the Visual Recognition Model
-When images are uploaded to both the negative and custom class you created(positive) status should read ready to train
-Click train model
![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic12.png)
![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic13.png)
![test](https://github.com/bmguillo/VisualRecognition/blob/master/img/pic14.png)


Additional Resources:
- [Getting Started Documentation](https://cloud.ibm.com/services/watson-vision-combined/crn%3Av1%3Abluemix%3Apublic%3Awatson-vision-combined%3Aus-south%3Aa%2F7d079bae5542b868586749125bad3e5b%3A719b0d28-22c9-489c-ae7b-2bfab84a857b%3A%3A?paneId=gettingStarted&new=true)
- [Visual Recognition API documentation](https://cloud.ibm.com/apidocs/visual-recognition)
- [Visual recognition CLI tools](https://developer.ibm.com/dwblog/2017/command-line-tools-watson-visual-recognition/)
- [Sharpening Visual Recognition Results using Tile Localization](https://www.ibm.com/cloud/blog/sharpen-watson-visual-recognition-results)
- [Redbook on Visual Recognition](http://www.redbooks.ibm.com/Redbooks.nsf/RedbookAbstracts/sg248393.html)
- [Guidelines for training custom classifiers](https://cloud.ibm.com/docs/services/visual-recognition?topic=visual-recognition-customizing)
- [Best practices for training custom classifiers](https://www.ibm.com/cloud/blog/watson-visual-recognition-training-best-practices)



