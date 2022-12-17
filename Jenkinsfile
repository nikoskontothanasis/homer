// The failedStages variable is reused between stages
def failedStages=[]
//Declarative
pipeline {
  agent { label "docker" }
  //parameters {}
    
  options {
    timeout(time: 1, unit: "HOURS")
  }
  
  stages {
        stage("Build & Deploy") {
            steps {
              sh "docker-compose up -d"
            }
        }
  }
}

