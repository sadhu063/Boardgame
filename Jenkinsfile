pipeline {    
    agent {
    label 'slave-1'
    }

 
     tools {
        maven 'MAVEN3'
        
    }

    

    stages {   
        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        
        stage('Build') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
