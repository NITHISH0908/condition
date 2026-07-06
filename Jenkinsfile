// when : atleast one condition must be specified

pipeline{
    agent any
    environment{
        DEPLY_TO = "production"
    }
    stages{
        stage('WhenStage'){
            when{
               environment name : 'DEPLY_TO', value: 'production'
            }
            steps{
                echo "Deploying to when stage"
            }

        }
    }
    }
}
