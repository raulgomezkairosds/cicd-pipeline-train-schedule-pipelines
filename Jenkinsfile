pipeline {
  agent
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh ./gradlew build --no-daemon
      }
    }
    stage('Results') {
      steps {
        archive 'dist/trainSchedule.zip'
      }
    }
  }
}
