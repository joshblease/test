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
      steps {
        sh 'echo "build"'
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
  }
}