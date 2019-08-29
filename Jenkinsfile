node {
   
   stage('Code Checkout') { // for display purposes
      git credentialsId: 'githubID', url: 'https://github.com/itrainarticle370simple-java-maven-app.git'
   }
   stage('Build') {
    withMaven(jdk: 'JDK-1.8', maven: 'Maven-3.6.1') {
     sh 'mvn clean compile'
     } 
   }
   stage('UnitTest run') {
    withMaven(jdk: 'JDK-1.8', maven: 'Maven-3.6.1') {
     sh 'mvn test'
     }   
   }
   stage('Code Quality') {
      
   }
   stage('Archival repo') {
    withMaven(jdk: 'JDK-1.8', maven: 'Maven-3.6.1') {
     sh 'mvn package'
     }   
   }
   stage('Docker Build') {
      
   }
   stage('Deploy to Dev') {
      
   }
   stage('Deploy to Prod') {
      
   }
   
}
