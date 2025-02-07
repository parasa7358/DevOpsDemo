pipeline {
    agent any
    
    stages {
         stage ('Clone') {
            steps {
                git branch: 'main', url: "https://github.com/parasa7358/DevOpsDemo.git"
            }
         }
        stage('Build') {
            steps {
                sh 'mvn -f onlinebookstore/pom.xml clean install'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn -f onlinebookstore/pom.xml test'
            }
            }

}
      }
