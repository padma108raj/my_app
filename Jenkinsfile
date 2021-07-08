node{
 stage('Checkout'){
    git 'https://github.com/padma108raj/my_app'
 }
 stage('Build-Package'){
  def mvnHome=tool name: 'maven-3', type: 'maven'
  sh "${mvnHome}/bin/mvn package"
 }
 stage('Send Mail Notification'){
  mail bcc: '', body: 'Check the build status', cc: '', from: '', replyTo: '', subject: 'Jenkins Notification', to: 'padma108raj@gmail.com'
 }
}
