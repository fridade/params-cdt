pipeline {
    agent any
    parameters {
      string description: 'Enter your first name ', name: 'firstName'
      string description: 'Enter your last name ', name: 'lastName'
    }


    stages {
        stage('welcome') {
            steps {
                echo "hi ${params.firstName} ${params.lastName}, welcome"
            }
        }
        stage('stage2') {
            steps {
                echo 'Hello World bonjour'
            }
        }
        stage('stage3') {
            steps {
                echo 'Hello World bonjour'
            }
            
        }
        stage('stage4') {
            steps {
                echo 'Hello World bonjour'
            }
            
        }
    }
}
    