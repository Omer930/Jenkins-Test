pipeline {
    agent any
    
    stages {
        stage('Image Build') {
            agent { dockerfile true }
            steps {
                sh 'node --version'
            }
        }
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
}

