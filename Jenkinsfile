pipeline {
    agent any
    stages {
        stage("Build"){
            steps {
                echo 'Building the application...'
                echo '...........................................................'
                sh 'npm install'
                sp 'npm run build'
            }
        }
        stage("Test") {
            steps {
                echo 'Testing the application...'
                echo '...........................................................'
                sp 'npm run test'
            }
        }
        stage("Deploy") {
            steps {
                echo 'Starting the service...'
                echo '...........................................................'
                sp 'npm run start'
            }
        }
    }
}