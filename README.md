##Learning Map Generator Setup Instructions

##Install Hugo

macOS: `$ brew install hugo`

To install on other platforms visit: `https://gohugo.io/`

##Check Hugo Version:

`$ hugo version`

##Clone Learning Map Generator

`$ git clone https://github.com/tyrin/learning-map-generator.git`

##Build the Site Locally. 
This step creates a public folder and copies all the static content & images. 
The site content will load from the public folder. To create the public folder run hugo without any arguments.

`$ hugo`

##Locally Load Static Site. 
This helps you visualize & validate what your site looks like

`$ hugo server`

Open browser and go to `http://localhost:1313`.

Press ctrl+c to stop the server.

##Deploy using Netlify
1. Go to https://app.netlify.com/
2. Connect your github account & pick your repo
3. Update Deploy Settings:
    - Base directory: `<your repo>`
    - Build command: hugo
    - Publish directory: `<your repo>/public`
    - Other setting pieces can remain in default state.
4. Save and deploy

Notes:
1. You can pick which branch will be used to deploy the site
2. You can customize the auto-deployment settings
3. Deploy logs are pretty useful if you want to debug deployment issues
4. Default, everytime a change is commited deployment is triggered.