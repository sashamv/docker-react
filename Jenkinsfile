pipeline {
    agent any
    stages {
        stage('Build Dev Env') {
            steps {
                echo 'Hello world!'
                sh "docker version"
                sh "docker build -t docker-react -f Dockerfile.dev ." 
                //sh "docker run -e CI=true docker-react npm run test -- --coverage"
            }
        }
        stage('Test') {
            steps {
               sh "docker run -e CI=true docker-react npm run test -- --coverage" 
            }
        }
    }
}
