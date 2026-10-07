pipeline{
agentany
tools{
maven'Maven3'
}
stages{
stage('Checkout') {
steps{
gitbranch: 'main', url: 'https://github.com/<your-username>/maven-package-demo.git'
}
}
stage('Package') {
steps{
bat 'mvncleanpackage'
}
}
stage('RunJAR') {
steps{
bat 'java-cptarget\\maven-package-demo-1.0.jarcom.example.App'
}
}