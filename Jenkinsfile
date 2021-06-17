pipeline {
    
    agent any

    stages {
        stage ('Deploy Master Branch') 
        {
            when 
            {
                expression { env.GIT_BRANCH == 'master' }
            }
            steps 
            {
                echo "Hello, origin/master"
            }
        }
        stage ('Deploy Develop Branch')
        {
            when 
            {
                expression { env.GIT_BRANCH == 'develop' }
            }
            steps 
            {
                echo "Hello, develop"
            }

        }
        stage('Deploy Tag') {
            when { tag "release-*" }
            steps {
                echo 'Deploying only because this commit is tagged...'
                sh 'make deploy'
            }
        }

    }
}