pipeline {
  agent {
    node {
      label 'ubuntu'
    }

  }
  stages {
    stage('Check prereq') {
      steps {
        sh 'kubectl get pods'
      }
    }

  }
}