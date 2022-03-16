pipeline {
    parameters {
        string defaultValue: 'defaultValue', name: 'testParameter'
    }
    agent any

    stages {
        stage('Clean WS') {
            steps {
                cleanWs()
            }         
        }
        stage('My Stage') {
            steps {
                echo 'Hello World'
                sh 'echo ${testParameter}'
                sh 'echo "Hello JENKINS Pipeline"'
            }
        }
    }
}
