pipeline {
    agent any
    parameters {
        string(name: 'NAME', description: 'Please tell me your name?')
        string(name: 'Address', description: 'Enter your address, for the pipeline trigger')
        text(name: 'DESC', description: 'Describe about the job details')
        choice(name: 'BRANCH', choices: ['Dev', 'Test', 'Stage','prod'], description: 'Choose one environment')
        
    }
    stages {
        stage('Printing Parameters') {
            steps {
                echo "Hello ${params.NAME}"
 
                echo "Job Details: ${params.DESC}"
 
                echo "Skip Running Test case ?: ${params.SKIP_TEST}"
 
                echo "Branch Choice: ${params.BRANCH}"
 
                echo "APP Password: ${params.SONAR_SERVER_PWD}"
            }
        }
    }
}
