node {

 stage('SCM checkout') {
   git 'https://github.com/medmedchiheb/devops-ci-simple'
 }
 stage('Build') {
  // get Maven home path
  def mvnHome = tool name: 'maven', type: 'maven'
  sh "${mvnHome}/bin/mvn clean install"
 }

}
