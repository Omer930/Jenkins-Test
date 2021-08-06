pipeline {
    agent any
    stages{
        stage('Host') {
            steps {
                nodejs('NodeJS'){
                    sh 'npm install'
                    sh' npm build'
                } 
            }
        }
        stage('Cloning our Git') { 
            steps { 
                git 'https://github.com/Annasali2/jenkins-test.git' 
            }
        
        
    }
}

