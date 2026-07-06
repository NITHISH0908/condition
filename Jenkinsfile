pipeline{
    agent any
    parameters{
        string(name: 'PERSON', defaultValue: 'nithish', description: 'Enter your name')
    }
    stages{
        stage('ParametersExample'){
            steps{
                 echo "welcome $(params.PERSON)"
            }
        }
    }
}
