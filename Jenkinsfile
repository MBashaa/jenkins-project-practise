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
        stage('default jenkins example env variables')
        {
            steps{
                echo "build number is:${env.BUILD_NUMBER}"
                echo "build id is:${env.BUILD_ID}"
                echo "build tag is:${env.BUILD_TAG}"
                echo "build executor is:${env.EXECUTOR}"
                echo "java path is:${env.JAVA_HOME}"
                echo "jenkins url is:${env.JENKINS_URL}"
                echo "job name is:${env.JOB_NAME}"
                echo "workspace is: ${env.WORKSPACE}"

            }
        }

    }


}