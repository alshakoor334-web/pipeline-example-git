pipeline{
    agent any

    stages{

        stage("compile"){
            steps{
               cmd /c 'javac Test.java'
            }
        }

        stage("run"){
            steps{
                cmd /c "java Test"
            }
        }

    }

    post{
        always{
            cmd /c 'echo "always"'
        }
        
        success{
            cmd /c 'echo "sucess"'
        }

        failure{
            cmd /c 'echo "failure"'
        }
    }


}