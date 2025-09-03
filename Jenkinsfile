/*pipeline
{
    agent any
     stages{
        stage('stage1')
        {
            steps{
                echo "global env with credenatils keyword"
                withCredentials([usernamePassword(credentialsId: 'user-cred', usernameVariable: 'myusername', passwordVariable: 'mypassword')])
                {
                    sh '''
                            ##echo "my credentials are "
                            ##echo "my username is: ${myusername}"
                            ##echo "my passowrd is: ${mypassword}"
                            
                            echo "my username is: $myusername"
                            echo "my password is: $mypassword"
                    '''
                }
            }
        }

        stage('stage2 logging in another ec2 instance')
        {
            steps{
                withCredentials([sshUserPrivateKey(credentialsId: 'ssh-key', keyFileVariable: 'my_ssh_key', usernameVariable: 'myuser' )])
                {
                    sh '''
                  
                    ssh -i $my_ssh_key -o strictHostKeyChecking=no ${myuser}@172.31.16.107 "hostname"


                    '''
                }
            }
        }
     }


}
*/

pipeline 
{
    agent any
    options{
        timeout(time: 1, unit: 'MINUTES')
        retry(2)
    }

    stages{

        stage('stage1'){
            steps{
                sh 'sleep 70'
            }
        }
    }
}