pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                echo 'Cloning repository...'
            }
        }

        stage('Build') {
            steps {
                echo 'Building project...'
                bat 'ren index.java CrudOperation.java || echo File rename skipped'
                bat 'javac CrudOperation.java'
                bat 'java CrudOperation'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing project...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying project...'
            }
        }
    }
}