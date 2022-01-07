pipeline 
{
    agent any

    stages 
    {
        stage('Build') 
        {
            steps 
            {
                echo 'Building..'
            }
        }
        stage('Test') 
        {
            steps 
            {
                echo 'Testing..'
            }
        }
        stage('Deploy') 
        {
            steps 
            {
                echo 'Deploying..'
            }
        }
    }
    post
    {
        always
        {
        emailext body: '''Hi,

        PFA URL,
        http://localhost:8080/job/MyFrirstPipeline/''', subject: 'Pipeline Status', to: 'zudhakar123@gmail.com'
        }
    }
}
