pipeline 
{
    agent any
    stages 
    {
        stage('Feature Pipeline') 
        {
            when 
            { 
                branch "feature-*" 
            }
            steps 
            {
                echo "*****************************"
                echo "sonar quality gate analysis"
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
                echo "release-1.0"
                echo "feature-1.0"
                echo "feature-2.0-bug"
                echo "feature-3.0"
                echo "*****************************"
            }
        }
        stage('QA Pipeline') 
        {
            when 
            { 
                branch "staging" 
            }
            steps 
            {
                echo "*****************************"
                echo "Deploying to qa environment"
                echo "sonar quality gate analysis"
                echo "release-1.0"
                echo "feature-1.0"
                echo "feature-2.0-bug"
                echo "feature-3.0"
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
                echo "release-1.0"
                echo "feature-1.0"
                echo "feature-2.0-bug"
                echo "feature-3.0"
                echo "*****************************"
            }
        }
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
                echo "release-1.0"
                echo "feature-1.0"
                echo "feature-2.0-bug"
                echo "feature-3.0"
                echo "*****************************"
            }
        }
        stage('Tagging Pipeline') 
        {
            when 
            { 
                tag "demo-release-*" 
            }
            steps 
            {
                echo "*****************************"
                echo "Deploying to demo environment"
                echo "sonar quality gate analysis"
                echo "release-1.0"
                echo "feature-1.0"
                echo "feature-2.0-bug"
                echo "feature-3.0"
                echo "*****************************"
            }
        }
    }
}