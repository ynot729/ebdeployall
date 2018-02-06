# ebdeployall
A small command line script to deploy to multiple AWS Elastic Beanstalk enviroments

###Requirements
You will need AWSCLI which requires python and the script is written in PHP so you will need that as well

###Installattion
  1.  Download
  2.  You might need to make it an executable `chmod a+x /path/to/ebdeployall`
  3.  You can put it on your `/usr/local/bin/` or link to your path to make it globaly available:

      `ln -s /path/to/downloaded/edeployall /usr/local/bin/or/similar/ebdeployall`

###Usage
After you do your eb init and your project is set up for `eb deploy` you can use `ebdeployall` and it will read all the enviroments on the application and deploy the default application version to all of them. It will do a dry run if the flag `--run` is not set which I recommend not using until everything looks good from the dry run.
