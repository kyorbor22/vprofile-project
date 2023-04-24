pipeline{
  agent any
  stages{
    stage('fetch code') {
    steps {
       git branch: 'paac', url: 'https://github.com/kyorbor22/vprofile-project.git'
    }
   }
   stage('Build') {
      steps {
        sh 'mvn install'
      }
    }
    stage('Test') {
      steps {
        sh 'mvn test'
      }
    }
  }
}
