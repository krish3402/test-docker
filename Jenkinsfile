// pipeline {
//     agent any

//     stages {
//         stage('Deploying React.js container to Kubernetes') {
//           steps {
//             script {
//               kubernetesDeploy(configs: "nginx.yaml", kubeConfig: [path: ''], kubeconfigId: '1fb96fcc-7c40-424f-94fb-6b1a6acc52a7')
//             }
//           }
//         }
//     }

//     post {
//         success {
//             // Actions to be performed when the pipeline is successful
//             echo 'Pipeline executed successfully!'
//         }

//         failure {
//             // Actions to be performed when the pipeline fails
//             echo 'Pipeline execution failed!'
//         }
//     }
// }
pipeline {

  agent any


  

   stages {

  //   stage('Clone repository') {

  //     steps {

  //       git 'https://github.com/krish3402/test-docker.git'

  //     }

  //   }

    
   

    stage('Deploy to Kubernetes') {

      steps {

        kubernetesDeploy(

          configs: 'nginx.yaml',

          kubeconfigId: 'testing'

        )

      }

    }

  }

}
