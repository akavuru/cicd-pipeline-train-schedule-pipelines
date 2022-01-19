pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running Buld Automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
