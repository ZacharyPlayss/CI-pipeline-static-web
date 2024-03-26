# Pipeline for static web page config.
The yml config file can be found in .github/workflows/static.yml. 
(Disclaimer this config file will only work on GITHUB since it makes use of actions.)

The pipeline will validate HTML and CSS files. Creates error logs in the artifacts tab of the pipeline run and publish to github pages when everything is valid.

## How do I use this pipeline myself ?
### Existing repository?
- Go to the root of your repository and paste in the static.yml file inside of ".github/workflows/" folder.

### New repository?
- Check root of your repository.
- If the .github folder exists folllow steps for existing repository.
- If this doesn't exist create a .github folder with a workflows folder inside of it and paste in the static.yml file from my repository.

### Github pages?
Don't forget to let the github pages be managed by the CI pipeline.
This ca be done in settings > pages and select Source : "Github actions"
