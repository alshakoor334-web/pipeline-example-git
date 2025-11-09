pipeline
{
    agent any

    environment{
       set VERSION_NAME ="1.35"
    }

    stages{

        stage("compile"){
            steps{
               bat 'javac Test.java'
               bat 'echo "${VERSION_NAME}"'
            }
        }

        stage("run"){
            steps{
                bat "java Test"
            }
        }

    }

    post{
        always{
            bat 'echo "always"'
        }
        
        success{
            bat 'echo "sucess"'
        }

        failure{
            bat 'echo "failure"'
        }
    }


}