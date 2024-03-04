pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'i want to build'
      }
    }

    stage('Test') {
      steps {
        echo 'i want to test'
      }
    }

    stage('Stage') {
      parallel {
        stage('Stage') {
          steps {
            echo 'i want to stage'
          }
        }

        stage('deploy') {
          steps {
            echo 'i want to operate'
          }
        }

        stage('Operate') {
          steps {
            echo 'i want to operate'
          }
        }

      }
    }

  }
}