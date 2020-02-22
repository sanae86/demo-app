node{
   stage('SCM Checkout'){
      git credentialsId: 'git-creds', url: 'https://github.com/sanae86/demo-app'
   }
   stage('Mvn Package'){
     def mvnHome = tool name: 'maven-3', type: 'maven'
     def mvnCMD = "${mvnHome}/bin/mvn"
     sh "${mvnCMD} clean package"
   }
  }
