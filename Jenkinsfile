pipeline {
  agent {
    label 'agent'
  }
    tools{
       maven 'maven'
    }

    stages {
        stage('scm') {
            steps {
                git branch:'master',url:'https://github.com/shreyadey16/sample1.git'
            }
        }
        stage('Build') {
            steps {
                sh ' mvn clean install'
            }
        }
      
    }
}
