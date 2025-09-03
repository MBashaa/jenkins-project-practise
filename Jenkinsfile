pipeline
{
    agent any
    environment{
        CRED = credentials('user-cred')
        
    }
    stages {
   
        stage('stage 1')
        {        
        steps{
                echo "printing credentials in stage1: ${CRED}"
             }         
        }

        stage('stage2')
        {
            steps{
                echo "username is: ${CRED_USR}"
                echo "password is: ${CRED_PSW}"
            }
        }

    }


}