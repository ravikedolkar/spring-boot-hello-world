pipeline {
    
    agent any

    stages {
        stage ('Deploy Master') 
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
        stage ('Deploy Develop')
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

    }
}