pipeline {
    
    agent any

    stages {
        stage ('Deploying Master') 
        {
            when 
            {
                branch "master" 
            }
            steps 
            {
                echo "Hello, origin/master"
            }
        }
        stage ('Deploying Develop')
        {
            when 
            {
                branch "develop"
            }
            steps 
            {
                echo "Hello, develop"
            }

        }
        stage('Deploy Tag') 
        {
            when 
            { 
                tag "release-*" 
            }
            steps 
            {
                echo 'Deploying only because this commit is tagged...'
            }
        }
    }
}