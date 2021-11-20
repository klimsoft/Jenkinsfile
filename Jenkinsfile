pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Build application with feature A'
            }
        }
        stage('Test') {
            steps {
                echo "Test application"
            }
        }
        stage('Deploy') {
            when {
                expression {
                    BRANCH_NAME == 'main'
                }
            }
            steps {
                echo "Deploy application"
            }

        }
    }
}