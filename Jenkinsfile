pipeline {
    agent any

    stages {
        stage('Example Stage') {
            steps {
                script {
                    // Some code or commands

                    // Print a message to the Jenkins console
                     echo testing
                    // More code or commands
                }
            }
        }
    }

    post {
        success {
            // Actions to be performed when the pipeline is successful
            echo 'Pipeline executed successfully!'
        }

        failure {
            // Actions to be performed when the pipeline fails
            echo 'Pipeline execution failed!'
        }
    }
}
