pipeline {
    agent any
    stages {
        stage("Build"){
            steps {
                echo 'Building the application...'
                echo '...........................................................'
                sh 'npm install'
                sp 'npm build'
            }
        }
        stage("Test") {
            steps {
                echo 'Testing the application...'
                echo '...........................................................'
                sp 'npm test'
            }
        }
        stage("Deploy") {
            steps {
                echo 'Starting the service...'
                echo '...........................................................'
                sp 'npm start'
            }
        }
    }
}