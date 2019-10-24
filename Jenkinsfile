pipeline {
    agent any 
    stages {
        stage('Fetch and Clean') { 
            steps {
                //clone git repo
                sh 'mvn clean'
            }
        }
        stage('Test') { 
            steps {
                // Test project
                sh 'mvn test'
            }
        }
        stage('Deploy') { 
            steps {
                // Package 
                sh 'mvn package'
            }
        }
    }
}
