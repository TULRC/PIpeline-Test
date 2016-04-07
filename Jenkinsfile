#!groovy

   stage 'Checkout'
   node {
   // Get code from a GitHub repository
   git url: 'https://github.com/Deepika-nagula/chef-repo.git'
   }

   // Get the maven tool.
   // ** NOTE: This 'M3' maven tool must be configured
   // **       in the global configuration.           
   def mvnHome = tool 'M3'

   // Mark the code build 'stage'....
   stage 'Build'
   // Run the maven build
   sh "${mvnHome}/bin/mvn clean install"
}
