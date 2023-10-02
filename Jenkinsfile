pipeline {
  agent any 
  tools {
    java 'java'
    maven 'maven'
  }
  stages {
    stage (Stage-1 Clean) {
      step {
        sh 'mvn clean'
      }
    }
    stage (Stage-2 Validate) {
      step {
        sh 'mvn validate'
      }
    }
    stage (Stage-3 Compile) {
      step {
        sh 'mvn compile'
      }
    } 
    stage (Stage-4 Task) {
      step {
        sh 'mvn task'
      }
    }
    stage (Stage-5 Package) {
      step {
        sh 'mvn package'
      }
    } 
    stage (Stage-6 Verify) {
      step {
        sh 'mvn verify'
      }
    }
    stage (Stage-7 Install) {
      step {
        sh 'mvn install'
      }
    }
  }
}
