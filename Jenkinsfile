pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git url: 'https://github.com/nareshh49/maven_pl-421.git'
                sh 'ls -lart'
                sh 'mvn package'
                
            }
        }
        stage('Test') {
            steps {
                sh 'ls -lart'
                sh 'mvn test'
            }
        }
        stage ('Run') {
            steps {
                sh 'ls -lart'
                sh 'java -cp target/maven-test3-1.0-SNAPSHOT.jar com.naresh.App'
    
           }
       }
        
    }
}

