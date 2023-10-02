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
 }
} 
