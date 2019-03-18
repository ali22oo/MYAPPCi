node{
   stage('SCM Checkout'){
       git credentialsId: 'creden1', url: 'https://github.com/ali22oo/MYAPPCi'
   }
        stage('Mvn Package'){
     def mvnHome = tool name: 'maven-3', type: 'maven'
     def mvnCMD = "${mvnHome}/bin/mvn"
     sh "${mvnCMD} clean package"
   }
   }

