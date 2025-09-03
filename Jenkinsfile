pipeline
{
    agent any
     stages{
        stage('stage1')
        {
            steps{
                echo "global env with credenatils keyword"
                withCredentials([userNamePassword(credentialsId: 'user-cred', usernameVariable: 'myusername', passwordVariable: 'mypassword')])
                {
                    sh '''
                            echo "my credentials are "
                            echo "my username is: ${myusername}"
                            echo "my passowrd is: ${mypassword}"

                    '''
                }
            }
        }
     }


}