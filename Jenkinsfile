
    pipeline{
        agent any
        stages{
            stage('Build'){
                steps{
                echo "Building the application"
                }
            }
            stage('sonar'){
                steps{
                echo "Building the sonar application"
                }
            }
            stage('DockerBuild'){
                steps{
                echo "Building the Docker file"
                }
            }
            stage('Dockerpush'){
                steps{
                echo "Pushing the docker image"
                }
            }
            stage('DeploytoDev'){
                steps{
                echo "deplying the application to Dev Env"
                }
            }
             stage('DeploytoTest'){
                steps{
                echo "deplying the application to Test Env"
                }
            }
             stage('Deploytostage'){
                when{
                    branch 'release/*'
                }
                steps{
                echo "deplying the application to stage Env"
                }
            }
             stage('DeploytoProd'){
                when{
                    tag pattern: "v\\d{1,2}\\.\\d{1,2}\\.\\d{1,2}", comparator: "REGEXP"
                }
                steps{
                echo "deplying the application to roduction Env"
                }
            }
        }
    }
