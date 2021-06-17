pipeline {
    
    agent any

    stages {
        stage ('Deploying To Production Environment') 
        {
            when 
            {
                branch "master" 
            }
            steps 
            {
                echo "release1"
                echo "feature1"
            }
        }
        stage ('Deploying To Develop Environment')
        {
            when 
            {
                branch "develop"
            }
            steps 
            {
                echo "release1"
                echo "feature1"
            }

        }
        stage('Deploying To QA Environment') 
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
        stage('Deploying To UAT Environment') 
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