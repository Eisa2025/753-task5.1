pipeline {
    agent any

    environment {
        DIRECTORY_PATH = 'C:\\Users\\thisi\\Downloads\\753\\753.5.1'
        TESTING_ENVIRONMENT = 'Testing'
        PRODUCTION_ENVIRONMENT = 'Your Name'
    }

    stages {
        stage('Build') {
            steps {
                echo "Fetch the source code from the directory path specified by the environment variable: ${DIRECTORY_PATH}"
                echo "Compile the code and generate any necessary artifacts"
            }
        }

        stage('Test') {
            steps {
                echo "Run unit tests"
                echo "Run integration tests"
            }
        }

        stage('Code Quality Check') {
            steps {
                echo "Check the quality of the code"
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploy the application to a testing environment specified by the environment variable: ${TESTING_ENVIRONMENT}"
            }
        }

        stage('Approval') {
            steps {
                sleep(time: 10, unit: 'SECONDS')
            }
        }

        stage('Deploy to Production') {
            steps {
                echo "Deploy the code to the production environment specified by the environment variable: ${PRODUCTION_ENVIRONMENT}"
            }
        }
    }
}