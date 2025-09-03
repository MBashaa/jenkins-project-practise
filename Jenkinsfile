pipeline
{
    agent any
    stages {

        stage('nested stage')
        {
            parallel{
                stage('inside stage 1')
                {
                    steps{
                        echo "first stage inside nested stage"
                    }
                }
                stage('inside stage 2')
                {
                    steps{
                        echo "second stage inside nested stage"
                    }
                }
            }
            
        }

        stage('stage2')
        {
            steps{
                echo "lets deep dive in jenkins"
            }
        }

    }


}