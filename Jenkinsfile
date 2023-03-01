pipeline {
    agent any

    stages 
    {
        stage('Build') 
        {
            steps 
            {
                echo 'This is to build an App'
            }
        }
        stage('Test') 
        {
            steps 
            {
                echo 'This is to test an App'
            }
        }
        stage('Deploy') 
        {
            steps 
            {
                echo 'This is to deploy an App'
            }
        }
    }
	post
	{
		always
		{
			emailext body: 'summary', replyTo: 'deepuprakashaj@gmail.com', subject: 'Pipeline-Notify', to: 'deepuprakashaj@gmail.com'
		}
	}
}
