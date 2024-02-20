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
        sh 'cd dev/hlf-operator/new'
        sh 'echo \'Hello world\''
      }
    }

  }
}