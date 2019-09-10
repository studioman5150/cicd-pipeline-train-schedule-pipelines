pipeline {
    agent any
    stages {
      stage ('build') {
       steps {
         echo 'Running build automation'
         sh './gradlew build --no-daemon'
         archiveArtifacts artifacts 'dists/trainSchedule.zip' 
       }
      }
    }
}
