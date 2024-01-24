pipeline {
    agent any

    stages {
        stage("Clone Repo"){
            steps {
                sh "docker --version" 
            }
        }
        stage("Clean Up"){
            steps {
                deleteDir()
                sh "ls -al" 
            }
        }
    }
    
}