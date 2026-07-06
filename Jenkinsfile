pipeline {

    agent any

    tools {
        maven 'Maven'
    }

    stages {

        stage('Clone Repository') {

            steps {

                git branch: 'main',
                url: 'https://github.com/Kusuma123-19/devops.git'

                echo "GitHub Repository Cloned Successfully134"
            }
        }

        stage('Build Project') {

            steps {

                sh 'mvn clean install'

                echo "Build Completed Successfully"
            }
        }

        stage('Test Project') {

            steps {

                echo "Testing Application"

                sh 'mvn test'
            }
        }

        stage('Deploy Project') {

            steps {

                echo "Deploying SaaS Project Management Tool"
            }
        }
    }

    post {

        success {

            echo "Pipeline Executed Successfully"
        }

        failure {

            echo "Pipeline Failed"
        }
    }
}