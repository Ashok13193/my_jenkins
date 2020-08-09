node{
  stage('GIT CHECKOUT') {
    git 'https://github.com/Ashok13193/my_jenkins.git'
 
  }
  stage('MAVEN BUILD'){
    def MAVEN_HOME =tool name: 'M3', type: 'maven'
    sh "${MAVEN_HOME}/bin/mvn package"
  
  }
  
  stage('Email Notification'){
    mail bcc: '', body: 'Hello, buddy this is from Jenkins', cc: '', from: '', replyTo: '', subject: 'Jenkins ALERT', to: 'gashok13193@gmail.com'
  }
   
}
