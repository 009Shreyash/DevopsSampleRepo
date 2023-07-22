pipeline{
  agent any
  stages{
    stage ('Compile Stage'){
      Steps {
        withMaven(maven : 'maven'){
          sh 'mvn clean compile'
        } 
      }
    }
    stage ('Test Stage'){
      Steps {
        withMaven(maven : 'maven'){
          sh 'mvn test'
        } 
      }
    }
    stage ('Deployment Stage'){
      Steps {
        withMaven(maven : 'maven'){
          sh 'mvn deploy'
        } 
      }
    }
  }
}
