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
/*        stage('Build Dev Dockerfile'){
            agent {
               dockerfile {
                   filename 'Dockerfile.dev' 
                }
            }
            steps {
               echo "Try to build image using a Dockerfile.dev file" 
               sh "docker build -t docker-react -f Dockerfile.dev ." 
            }
        }*/
    }
}
