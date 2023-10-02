pipeline {
  agent any 
  tools {
    jdk 'java'
    maven 'maven'
  }
  stages {
    stage ('Stage-1 Clean') {
      steps {
        sh 'mvn clean'
      }
    }
    stage('Stage-2 Validate') {
      steps {
        sh 'mvn validate'
      }
    }
    stage('Stage-3 Compile') {
      steps {
        sh 'mvn compile'
      }
    } 
    stage('Stage-4 Package') {
      steps {
        sh 'mvn package'
      }
    } 
    stage('Stage-5 Verify') {
      steps {
        sh 'mvn verify'
      }
    }
    stage('Stage-6 Install') {
      steps {
        sh 'mvn install'
      }
    }
  }
}
