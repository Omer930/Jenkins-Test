pipeline {
    agent any
    
    stages {
        stage('Image Build') {
            agent { dockerfile true }
            steps {
                sh 'node --version'
            }
        }
        stage('Build') {
            steps {
                nodejs('NodeJS'){
                    sh 'npm install'
                    sh' npm build'
                } 
            }
        }
        stage('Cloning our Git') { 
            steps { 
                git '' 
            }
        } 
        
    }
}
    

