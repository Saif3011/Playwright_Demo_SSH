pipeline {
    agent any

    stages {
        stage('Build test') {
            steps {
                npm install
                npm init playwright@latest
            }
        }
         stage('Run test') {
            steps {
                npx playwright test ./tests/APITest.spec.js
            }
        }
         stage('Deploy test') {
            steps {
                echo 'I am deploying test'
            }
        }
        stage('Sending message') {
            steps {
                echo 'I am sending a message'
            }
        }
    }
}
