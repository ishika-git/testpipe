pipeline{
 agent any
   stages{
     stage('checkout'){
         steps{
                checkout scm
              }}
     stage('Build'){
         steps{
                sh '/home/ishika/Documents/devops_software/apache-maven-3.9.6/mvn install'
              }}
     stage('Deployment'){
         steps{
                sh 'cp target/testpipe.war /home/ishika/Documents/devops_software/apache-tomcat-9.0.85/webapps'
              }}
}}
