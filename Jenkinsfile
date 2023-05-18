pipeline {
    agent any
 options {
        timeout(time: 1, unit: 'MINUTE')
 }
  stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
        stage('DONE') {
            steps {
                echo 'SUCESS....'
            }
        }
    }
}
