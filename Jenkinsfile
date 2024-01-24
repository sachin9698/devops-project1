pipeline {
    agent any

    stages {
        stage("Clone Repo"){
            steps {
                sh "docker ps" 
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