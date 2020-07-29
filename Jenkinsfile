node{
  stage('GIT CHECKOUT') {
    git 'https://github.com/Ashok13193/my_jenkins.git'
 
  }
  stage('MAVEN BUILD'){
    def MAVEN_HOME =tool name: 'M3', type: 'maven'
    sh "${MAVEN_HOME}/bin/mvn package"
  
  }
   
}
