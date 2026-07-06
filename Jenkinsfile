pipeline {

    agent any

    stages {

        stage('Clone') {

            steps {

                echo "GitHub Connected Successfully"
            }
        }

        stage('Build') {

            steps {

                echo "Build Started1"
            }
        }

        stage('Deploy') {

            steps {

                echo "Deployment Successful"
            }
        }
    }

    post {

        success {

            echo "Pipeline Executed Successfully"
        }

        failure {

            echo "Pipeline Failed1"
        }
    }
}