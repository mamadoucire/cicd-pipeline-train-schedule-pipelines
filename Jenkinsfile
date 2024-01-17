pipeline {
  agent any
  stages{
    stage('buid') {
      steps {
        echo "running build automation"
        sh './gradlew build --no-daemon'
        archivesArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
