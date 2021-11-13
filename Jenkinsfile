pipeline {
  agent any
  tools {
    maven 'maven383'
  }
  stages {
    stage('checkout') {
      steps {
        checkout scm
      }
    }
    stage('build') {
      steps {
        sh "mvn clean install"
      }
    }
  }
}






/* #!groovy

pipeline {
  agent none
  stages {
   
    stage('Docker Build') {
      agent any
      steps {
        sh 'docker build -t centos:latest .'
      }
}
     stage('Docker Run') {
      agent any
      steps {
        sh 'docker run -dit -p 8082:80 centos'
      }
     
    }
  }
}
*/
