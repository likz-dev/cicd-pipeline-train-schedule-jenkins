pipeline { 
  agent any // Restrict which agent the agent can run on 

  stages {
    stage ('Build') { 
      steps { 
        echo 'Running build automation'
        sh './gradlew build --no-daemon' // Turns of the gradle daemon
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  } 
}
