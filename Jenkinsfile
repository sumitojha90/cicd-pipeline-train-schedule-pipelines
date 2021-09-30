pipeline {

  agent any
  
  stages {
  
    stage ('Build'){
      steps {
        echo 'Running build automation'
        sh 'gradle wrapper'
        sh '/.gradlew build'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  
  }
  
}
