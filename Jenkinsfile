pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'This is a new build'
          }
        }

        stage('build engine') {
          steps {
            echo 'Build Engine'
          }
        }

        stage('Build Body') {
          steps {
            echo 'Build Body'
          }
        }

      }
    }

    stage('Flash ECU') {
      steps {
        echo 'Flash ECU'
      }
    }

    stage('Run Test') {
      steps {
        echo 'ECU Test'
      }
    }

  }
}