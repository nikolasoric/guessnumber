pipeline {
  
  agent any
  
  stages {
  
    stage("run frontend") {
      
      steps {
        echo 'executing yarn...'
        nodejs('Node-10.17') {
          sh 'yarn install'
        }
      }
    }
    
    stage("no backend") {
      
      steps {
        echo 'gradle cant be executed, maybe beacuse the app is javascript and doesnt have gradle inside?...'
        }
      }
    }
  }
}
