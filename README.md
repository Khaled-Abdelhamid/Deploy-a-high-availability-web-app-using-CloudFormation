# Deploy-a-high-availability-web-app-using-CloudFormation
This is a project focusing on building infrastructure as code in AWS



## Folders and files

* infrastructure: The folder containing all cloudFormation configuration files to build the app.
  * create.sh:  a shell script to easily create cloudFormation stack.
  * update.sh:  a shell script to easily update cloudFormation stack.
  * kill.sh:  a shell script to easily delete cloudFormation stack.
* screenshots: The folder containing screen shots of stack creation events and outputs.

## stack creation steps:

1. Go to infrastructure folder

2. create network infrastructure using the following command:

   ```bash
   ./create.sh udagram-network network.yml network-params.json 
   ```

   

3. create server resources using the following command:

   ```bash
   ./create.sh udagram-servers servers.yml server-parameters.json
   ```



4. To check if the server is working or not, go to the following link:

   http://udagr-webap-erav97ltwa1f-2144831197.us-east-1.elb.amazonaws.com/
