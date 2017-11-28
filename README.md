README:

The release-to-npm can be used to publish images to npm. 

The below pipeline configuration demonstrates simple usage:


    deploy_to_npm:  
      title: Publishing To Npm 
      image: codefresh/release-to-npm
      commands:
      - NPM_TOKEN=${{NPM_TOKEN}} npm run ci-publish 


Parameter Reference:

    NPM_TOKEN : token of npm account
    
for getting the NPM_TOKEN please see https://docs.npmjs.com/private-modules/ci-server-config#getting-an-authentication-token
