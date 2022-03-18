pipeline {
    agent any
	

 stages {
      stage('checkout') {
           steps {
             
                git branch: 'main', url: 'https://github.com/suman7799/devops-practical-2.git'
             
          }
        }
       

  stage('Docker Build and Tag') {
           steps {
              
                sh 'docker build -t devopsclass:latest .' 
                sh 'docker tag devopsclass 8249355606/devopsclass:$BUILD_NUMBER'
               
          }
        } 
    }
}
