pipeline {
    agent any

    stages {
        stage('Deploy to Kubernetes') {
            steps {
                // Deploy to Kubernetes
                script {
                       kubernetesDeploy configs: 'nginx.yaml', kubeConfig: [path: ''], kubeconfigId: '1fb96fcc-7c40-424f-94fb-6b1a6acc52a7', secretName: '', ssh: [sshCredentialsId: '*', sshServer: ''], textCredentials: [certificateAuthorityData: '', clientCertificateData: '', clientKeyData: '', serverUrl: 'https://']
                }
            }
        }
    }

    post {
        success {
            // Perform actions when the deployment succeeds
            echo 'Deployment to Kubernetes successful!'
        }

        failure {
            // Perform actions when the deployment fails
            echo 'Deployment to Kubernetes failed!'
        }
    }
