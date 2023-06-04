pipeline {
    agent any
    environment{
        microcare ='academy'
        GIT_CRED = credentials('github') //username:password //secretkey
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
               //  def password = ${GIT_CRED_PSW}
             //  sh 'echo %env.GIT_CRED%'
             // echo "${password}"
                echo "${env.GIT_CRED_USR}"
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
