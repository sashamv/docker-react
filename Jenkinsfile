pipeline {
    agent any
    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello world!'
                sh "docker version"
                sh "hostname -f"
            }
        }
        stage('Build Dev Dockerfile'){
            agent {
                dockerfile {
                   filename 'Dockerfile.dev' 
                }
            }
            steps {
               sh "hostname -f" 
            }
        }
    }
}
