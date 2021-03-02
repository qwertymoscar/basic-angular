pipeline {
  agent any
  stages {
    stage('stage 1') {
      steps {
        echo 'TEsting step1'
      }
    }

    stage('stage 2.1') {
      parallel {
        stage('step 2.1') {
          steps {
            sh 'echo \'Test 2.1\''
          }
        }

        stage('stage 2.2') {
          steps {
            echo 'step 2.2 parallel'
          }
        }

      }
    }

  }
}