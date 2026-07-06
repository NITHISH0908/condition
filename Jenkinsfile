

pipeline{
    agent any
    stages{
        stage('Build'){
           echo "building the application"
        }
stage('DEPLOTTOPROD'){
    when{
        expression {BRANCH_NAME==~ /{production|staging}/}
    }
    steps{
        echo "deplying to Prod"
    }
}
    }
}
