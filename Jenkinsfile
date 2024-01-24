pipeline {
    agent any

    stages {
        stage("docker cleanup"){
            steps {
                sh "docker rm -f custom-web1"
                sh "docker image rm -f custom-web:v1"
            }
        }
        stage("docker build"){
            steps {
                sh "docker build -t custom-web:v1 ."
                sh "docker run --name custom-web1 -d -p 8081:80 custom-web:v1"
            }
        }
        stage("docker deploy"){
            steps {
                sh "docker run --name custom-web1 -d -p 8081:80 custom-web:v1"
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