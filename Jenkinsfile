pipeline {
agent any
tools {
maven 'Maven3'
}
stages {
stage('Build') {
steps {
dir('cicd-demo'){
bat 'mvn clean install'
}
}
}
stage('Test') {
steps {
dir('cicd-demo'){
bat 'mvn test'
}
}
}
}
}