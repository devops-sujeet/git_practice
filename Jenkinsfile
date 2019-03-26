@('Var-Lib)'_

pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
        stage('varlib') {
            steps{
                Myclass
            }
        }   
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
    }
}
