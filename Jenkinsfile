pipeline {
  
  agent any
  
  stages {
  
    stage("run frontend") {
      
      steps {
        echo 'executing yarn...'
        nodejs('Node-10.17') {
          batch 'yarn install'
        }
      }
    }
    
    stage("run backend") {
      
      steps {
        echo 'executing gradle...'
        withGradle(){
          batch './gradlew -v'
        }
      }
    }
  }
}
