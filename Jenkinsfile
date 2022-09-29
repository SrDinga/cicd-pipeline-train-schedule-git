pipeline {
  agent any
  stages {
    stage ('Build'){
      steps {
        echo 'Runinig Build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
