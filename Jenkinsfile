// #!/usr/bin/env groovy
// pipeline {
//     agent any
//     stages {
//         stage('Stage 1'){
//             steps{
//                 echo "hola mundo prueba"
//             }
//         }
//     }
// }

pipeline {
   agent any 
  
    stages {
        stage('Stage 1'){
            steps{
                echo "Prueba 2"
            }
        }
        stage('Build and Deploy ') {
            steps {
                sh '''docker-compose up -d build'''
            }
        }

        
        
    
    }
}

