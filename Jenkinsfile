pipeline {
    agent any    
    stages {      
          stage('Cloning our Git') { 
            steps { 
                git 'https://github.com/Omer930/Jenkins-Test.git' }
            }
        stage('Build') {
            steps {
                nodejs('NodeJS'){
                    sh 'npm install'
                    sh 'npm build'  } 
            }
         }
      
        } 
  
    

