pipeline {
    agent any
    parameters {
        string(name: 'GREETING',
        defaultValue: 'Hello', 
        description: 'The greeting message')
        choice(
            name: 'BRANCH',
            choices: ['master','development', 'dev222'],
            description : 'Branch kodu do vyboru'
            )
        
    }
    stages {
        stage('Example') {
            steps {
                echo "${params.GREETING}, we are building the ${params.BRANCH} branch."
            }
        }
    }
}

