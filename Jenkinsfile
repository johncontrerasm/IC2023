pipeline{
    agent any

    stages{
        stage('docker build'){
            steps{
                script{
                    "docker build -f 02-primer-pipeline/Dockerfile -t johncontrerasm/holamundo IC2023"
                }
            }
        }

        stage('docker push'){
            steps{
                script{
                    sh "docker push johncontrerasm/holamundo"
                }
            }
        }
    }

}

