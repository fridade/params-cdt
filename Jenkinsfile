pipeline {
    agent any
    parameters {
      string description: 'Enter your first name ', name: 'firstName'
      string description: 'Enter your last name ', name: 'lastName'
      choice choices: ['dev', 'qa', 'prod'], description: 'choose the env where you want the build to happen', name: 'Environment'

    }


    stages {
        stage('welcome') {
            steps {
                echo "hi ${params.firstName} ${params.lastName}, welcome"
            }
        }
        stage('deploy to dev') {
            when {
                expression {
                    params.Environment == "dev"
                }
            }
            steps {
                echo 'Hello World bonjour dev'
            }
        }
        stage('deploy to qa') {
            when {
                expression {
                    params.Environment == "qa"
                }
            }
            steps {
                echo 'Hello World bonjour qa'
            }
            
        }
        stage('deploy to prod') {
            when {
                expression {
                    params.Environment == "prod"
                }
            }
            steps {
                echo 'Hello World bonjour prod'
            }
            
        }
    }
}
    