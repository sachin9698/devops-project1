pipeline {
    agent any

    stages {
        stage("Clone Repo"){
            steps {
                sh "docker images" 
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