pipeline {
    agent any
    environment{
        microcare ='academy'
        devops ='customvariables'
    }
    stages {
        stage('Build') {
            steps {
               // echo "${USER}"
          bat('set')
            }
        }
         stage('Build1') {
            steps {
                echo "${env.microcare}"
                echo "${env.devops}"
            }
        }
         stage('Build2') {
              when{
                  not {
                 branch "master"
                  }
             }
            steps {
                echo 'Building..'
            }
        }
         stage('Build3') {
             when {
                 not{
                branch "devops"
                 }
             }
            steps {
                echo 'Building..'
            }
        }
    }
    post { 
        aborted { 
            echo 'ABORTED'
        }
         success { 
            echo 'SUCCESS'
        }
         failure { 
            echo 'FAILURE'
        }
        changed { 
            echo 'FAILURE'
        }
    }
    
}
