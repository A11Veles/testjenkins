pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    docker.build('my-docker-image')
                    sh 'git --version'

                }
            }
        }
        stage('Test') {
            steps {
                script {
                    docker.image('my-docker-image').inside {
                        sh 'echo "Running tests..."'
                    }
                }
            }
        }
    }
}
