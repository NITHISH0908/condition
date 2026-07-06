// when : atleast one condition must be specified

pipeline{
    agent any
    environment{
        DEPLOY_TO = "production"
    }
    stages{
        stage('WhenStage'){
            when{
               environment name : 'DEPLOY_TO', value: 'production'
            }
            steps{
                echo "Deploying to when stage"
            }

        }
    }
    }

