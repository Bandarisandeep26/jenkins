pipeline {
    // agent any
   agent {
        docker { 
            image 'maven:3.8.8' 
        }
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn --version'
                echo 'Build'
            }
        }
        stage('Test') {
            steps {
                echo 'Test'
            }
        }
        stage('Integration Test') {
            steps {
                echo 'Integration Test'
            }
        }
    }

    post {
        always {
            echo 'I always run Awesome'
        }
        success {
            echo 'I run when you are success'
        }
        failure {
            echo 'I run when you failed'
        }
    }
}
