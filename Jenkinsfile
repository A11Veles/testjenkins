pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    sh 'docker build -t test1 .'

                }
            }
        }
        // stage('Test') {
        //     steps {
        //         script {
        //             docker.image('my-docker-image').inside {
        //                 sh 'echo "Running tests..."'
        //             }
        //         }
        //     }
        // }
    }
}
