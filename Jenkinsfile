pipeline {
    agent none
    stages {
        stage('Beginning') { agent any
            steps {
                echo "hello world"
            }
        }
        stage('Who Am I?') { agent any
            steps {
               sh 'host -t TXT pgpmichaelholler.us |awk -F \'"\' \'{print 2}\'' 
            } 
        }
    }
}