pipeline{
    agent { label 'linux' }
    tools { maven 'M3' }
    stages{
       stage('checkout'){
          steps{
             git 'https://github.com/effectivejenkins/myProject.git'
             }
           }
       stage('Build'){
          steps{
            sh 'mvn clean compile'
            }
          }
        stage('package'){
           steps{
             sh 'mvn package'
           }
             }        
         
}
