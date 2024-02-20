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

    stage('Clean Environment') {
      steps {
        
        script{
          
        def dirname = 'hlf-operator'
        def directory = new File(dirname)
        
        if(directory.isExists() && directory.isDirectory()){
          directory.deleteDir()
          echo '$dirname existed and is deleted'
        }
        else{
          echo 'Directory $dirname does not exists'
        }
        
        mkdir $dirname
        
        
        }
      }
    }

  }
}