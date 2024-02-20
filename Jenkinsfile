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

    stage('Create Kind Cluster') {
      steps {
        sh 'mkdir hlf-operator && cd hlf-operator'
        sh 'echo \'Hello world\''
      }
    }

  }
}