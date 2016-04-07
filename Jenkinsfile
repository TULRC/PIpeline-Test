#!groovy

   stage 'Checkout'
   node {
   // Get code from a GitHub repository
   git url: 'https://github.com/Deepika-nagula/chef-repo.git'
   }

   stage 'Build'
   node {   
   // Run the maven build
   sh "${mvnHome}/bin/mvn clean install"
   }
