pipeline {
    
    agent any

    stages {
        stage ('Master Pipeline') 
        {
            when 
            {
                branch "master" 
            }
            steps 
            {
                echo "*****************************"
                echo "Deploying to prod environment"
                echo "sonar quality gate analysis"
                echo "release1.0"
                echo "feature1.0"
                echo "*****************************"
            }
        }
        stage ('Develop Pipeline')
        {
            when 
            {
                branch "develop"
            }
            steps 
            {
                echo "*****************************"
                echo "Deploying to dev environment"
                echo "sonar quality gate analysis"
                echo "release1.0"
                echo "feature1.0"
                echo "*****************************"
            }

        }
        stage('Feature Pipeline') 
        {
            when 
            { 
                branch "feature*" 
            }
            steps 
            {
                echo "*****************************"
                echo "sonar quality gate analysis"
                echo "*****************************"
            }
        }
        stage('Tagging Pipeline') 
        {
            when 
            { 
                tag "tag-release-*" 
            }
            steps 
            {
                echo "*****************************"
                echo "Deploying to qa environment"
                echo "sonar quality gate analysis"
                echo "release1.0"
                echo "feature1.0"
                echo "*****************************"
            }
        }
        stage('Release Pipeline') 
        {
            when 
            { 
                branch "release-*" 
            }
            steps 
            {
                echo "*****************************"
                echo "Deploying to uat environment"
                echo "sonar quality gate analysis"
                echo "release1.0"
                echo "feature1.0"
                echo "*****************************"
            }
        }
    }
}