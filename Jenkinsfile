pipeline {
    agent any

    stages {
        stage('Build and push api-tests image') {
            steps {
                echo 'Building api-tests docker image'

                sh 'docker build -t vnikolajevs/api-tests:latest .'

                echo 'Pushing image to docker hub'

                sh 'docker push vnikolajevs/api-tests:latest'
            }
        }
    }
}