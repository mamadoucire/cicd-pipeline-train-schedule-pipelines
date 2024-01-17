pipeline {
  agent any
  stages{
    stage('buid') {
      steps {
        echo "running build automation"
        sh 'gradle wrapper'
        sh './gradlew build --no-daemon'
        archivesArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
