pipeline{
    agent any

    stages{
        stage('docker build'){
            steps{
                script{
                    "docker build -f 02-primer-pipeline/Dockerfile -t admin/holamundo::1.0.0-${BUILD_ID} IC2023"
                }
            }
        }

        stage('docker push'){
            steps{
                script{
                    sh "docker push admin/holamundo:1.0.0-${BUILD_ID}"
                }
            }
        }
    }

}

