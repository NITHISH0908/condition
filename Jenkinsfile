
pipeline{
    agent any
    parameters{
        string(name: 'CHANGE_TICKET', defaultValue: 'CH12345', description: 'Enter the Change ticket Number')
        booleanParam(name: 'Is SRE Approved?', defaultValue: true, description: 'Is Approval taken')
        choice(choices:'Regular\nHotfix', description: 'what release is this', name: 'RELEASE')
        password(name:'myPassword', description:'Enter the password', defaultValue:Nani)
        credentials(name : 'mycreds', description: 'MyDockercreds', required: true)
    }
        stages{
            stage('DeploToStage'){
                steps{
                    echo "Deploy to Satge"
                }
            }
            stage('DeploToProd'){
                steps{
                    echo "your change ticket ${params.CHANGE_TICKET} has beem approved"
                    echo "Deploy to Prod"
                    echo "This is a ${params.RELEASE}"
                    echo "The password is ${params.myPassword}"
                    echo "selected creetails are ${params.mycreds}"
                }
            }

        }
    
}
