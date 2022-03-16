pipeline {
    parameters {
        string defaultValue: 'defaultValue', name: 'testParameter'
    }
    agent any

    stages {
        
        stage('My Stage') {
            steps {
                echo 'Hello World'
                sh 'echo ${testParameter}'
                sh 'echo "Hello JENKINS Pipeline"'
            }
        }
        stage('Execute Shell') {
            agent{
                label 'built-in'
            }
            steps {
                sh 'ls'
                sh 'chmod +x HelloWorld.sh'
                sh './HelloWorld.sh'
            }
        }
        stage('Clean WS') {
            steps {
                cleanWs()
            }         
        }
    }
}
