node{
 stage('Checkout'){
    git 'https://github.com/padma108raj/my_app'
 }
 stage('Build-Package'){
  def mvnHome=tool name: 'maven-3', type: 'maven'
  sh "${mvnHome}/bin/mvn package
 }
}
