pipeline {
    agent any

    stages {
        stage("Clone Repo"){
            steps {
                sh "ls -al" 
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