pipeline{
    agent none
    stages{
       stage('example build'){
          agent{ docker 'maven:3-alpine'}
          steps{
             echo 'Hello maven'
             sh 'mvn --version'
             }
           }
       stage('Example test'){
          agent { docker 'openjdk:8-jre' }
          steps{
            sh 'java -version'
            }
          }
 }        
}
