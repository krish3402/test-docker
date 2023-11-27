pipeline {
    agent any

    stages {
        stage('Example Stage') {
            steps {
                script {
                    // Some code or commands

                    // Print a message to the Jenkins console
                    kubernetesDeploy configs: 'nginx.yaml', kubeConfig: [path: ''], kubeconfigId: '1fb96fcc-7c40-424f-94fb-6b1a6acc52a7', secretName: '', ssh: [sshCredentialsId: '*', sshServer: ''], textCredentials: [certificateAuthorityData: '', clientCertificateData: '', clientKeyData: '', serverUrl: 'https://']

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
