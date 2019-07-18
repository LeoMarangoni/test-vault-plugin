pipeline {

    agent {
      label 'slave2'
    }


    stages {
      stage('Echo Start') {
        steps {
         sh "echo Start" 
        }
      }

      stage ('Echo Envs') {
        steps {
          sh "echo $VAULT_ADDR"
          sh "echo $V_SECRET"
        }
      }

      stage ('Echo End') {
        steps {
          sh "echo Ending"
        }
      }
    }
}
