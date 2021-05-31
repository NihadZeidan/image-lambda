# image-lambda


## Process:
 - I created a function in the AWS lambda and give it a name.
 - I added to the function .zip file that holds all the function files and packages.
 - I added a trigger that will trigger this lambda function.
 - That trigger will be connected to S3 service.
 - I created S3 bucket to connect this lambda function with.
 - Then whenever you upload an image in that bucket it will trigger the event and will call the lambda function.


## issues:
 - when I tried to upload the lambda function without node_modules folder it keep log an error saying `can not require async module: not Found`, So I uploaded all the node_modules to the lambda function as a zip file.