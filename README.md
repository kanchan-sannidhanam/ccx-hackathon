# ccx-hackathon

#Install Hugo:
macOs: $ brew install hugo
To install on other platforms visit: https://gohugo.io/

#Check version:
$ hugo version

#Clone Learning Map Generator
$ git clone https://github.com/tyrin/learning-map-generator.git

#Build the site locally. This step will create a public folder where all the static content & images will copied to. 
#The site content are loaded from the public folder
hugo

#Locally load the static site. This helps you visualize & validate what your site looks like
$ hugo server
open browser and go to http://localhost:1313
press ctrl+c to stop the server

#Deploy using Netlify
1. go to https://app.netlify.com/
2. Connect your github account & pick your repo
3. Update Deploy Settings:
    - Base directory: <your repo>
    - Build command: hugo
    - Publish directory: <your repo>/public
    - Other setting pieces can remain in default state.
4. Save and deploy

Notes:
1. You can pick which branch will be used to deploy the site
2. You can customize the auto-deployment settings
3. Deploy logs are pretty useful if you want to debug deployment issues
4. Default, everytime a change is commited deployment is triggered.