pipeline
{
    agent any
    environment{
        USER_NAME = "basha"
        PWD = "pass123"
        
    }
    stages {
   
        stage('stage 1')
        {        
        steps{
                echo "printing username in stage1: ${USER_NAME}"
             }         
        }

        stage('stage2')
        {
            steps{
                echo "printing username in stage 2 as well: ${USER_NAME} and his password is: ${PWD}"
                echo "these are called global environment variables can be applicable for all stages"
            }
        }

    }


}