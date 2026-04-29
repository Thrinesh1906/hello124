pipeline {
agent any
tools {
maven 'Maven3'
}
stages {
stage('CHECKOUT') {
steps {
git 'https://github.com/Thrinesh1906/hello124.git'
}
}
stage('Build') {
steps {
dir('demo'){
bat 'mvn clean install'
}
}
}
stage('Test') {
steps {
dir('demo'){
bat 'mvn test'
}
}
}
}
}