pipeline {
    parameters {
        string defaultValue: 'defaultValue', name: 'testParameter'
    }
    agent any

    stages {
        stage('TTTTT') {
            steps {
                echo 'Hello World'
              sh 'echo ${testParameter}'
                sh 'echo "Hello JENKINS Pipeline"'
            }
        }
    }
}
