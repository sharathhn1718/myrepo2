pipeline {
    agent any  // This will run the pipeline on any available agent
    
    stages {
        stage('Build') {
            steps {
                // Your build steps go here. For example, if you're using a build.ps1 script:
                echo 'Build stage succeeded'
                echo 'this is my build step 2'
            }
        }

        stage('Test') {
            steps {
                // Your test steps go here. For example, if you have a test.ps1 script:
                echo 'Test stage succeeded'
                echo 'this is my test step 2'
            }
        }

        stage('Deploy') {
            steps {
                // Your deployment steps go here. For example, if you have a deploy.ps1 script:
                echo 'Deploy stage succeeded'
                echo 'this is my deploy step 2'
            }
        }
    }

    post {
        always {
            // This block will always execute, regardless of the pipeline success/failure
            echo 'This will always run (ABS)'
        }

        success {
            // This block will only execute if the pipeline was successful
            echo 'Pipeline was successful! (ABS)'
        }

        failure {
            // This block will only execute if the pipeline failed
            echo 'Pipeline failed.(ABS)'
        }
    }
}
