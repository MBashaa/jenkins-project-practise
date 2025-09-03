pipeline
{
    agent any
    stages {
   
        stage('stage 1')
        {
            environment{
                USER_NAME = "basha"
                PASS_WORD = "password123"
            }

        steps{
                echo "Hi I am ${USER_NAME} my password is: ${PASS_WORD}"
             }         
        }

        stage('stage2')
        {
            steps{
                echo "User in stage1 is : ${USER_NAME}"
            }
        }

    }


}