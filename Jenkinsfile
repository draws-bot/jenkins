pipeline {
    agent {
        label 'AGENT-1'
    }
        parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

        text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')

        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo this is build'
            }
        }
        stage('Test') {
            steps {
                sh 'echo this is test'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo this is deploy'
            }
        }
    }
}