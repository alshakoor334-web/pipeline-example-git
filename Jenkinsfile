pipeline{
    agent any

    stages{

        stage("compile"){
            steps{
               sh 'javac Test.java'
            }
        }

        stage("run"){
            steps{
                sh "java Test"
            }
        }

    }

    post{
        always{
            sh 'echo "always"'
        }
        
        success{
            sh 'echo "sucess"'
        }

        failure{
            sh 'echo "failure"'
        }
    }


}