pipeline {
    agent {label 'micro'}
 options {
        // Timeout counter starts AFTER agent is allocated
    
        timeout(time: 1, unit: 'minute')
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
