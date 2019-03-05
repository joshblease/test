pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('Clean') {
      parallel {
        stage('Clean Scala') {
          steps {
            sh 'echo "Clean"'
          }
        }
        stage('Clean Java') {
          steps {
            sh 'echo "Clean"'
          }
        }
      }
    }
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'echo "build"'
          }
        }
        stage('') {
          steps {
            sh 'echo "1"'
          }
        }
      }
    }
    stage('Deploy ') {
      parallel {
        stage('PolandPL') {
          steps {
            sh 'echo "Deploy 1"'
          }
        }
        stage('Pre-Live') {
          steps {
            sh 'echo "Deploy 1"'
          }
        }
        stage('Stable') {
          steps {
            sh 'echo "Deploy 1"'
          }
        }
      }
    }
    stage('We wait') {
      steps {
        input 'Hello?'
      }
    }
    stage('End!') {
      steps {
        sh 'echo "DONE"'
      }
    }
  }
}