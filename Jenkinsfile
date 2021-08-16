pipeline {
    agent any
    
    stages {
        stage('SCM checkout') {
            steps {
                checkout scm: [$class: 'GITSCM',userRemoteConfigs: [[credentialsId: 'github-ssh-key', url: 'git@github.com:Digital-sam/declarative_CICD.git']]]
            }
        }
        
        stage('test') {
            steps {
                echo 'This is the test stage'
            }
        }
        stage('deploy') {
            steps {
                echo 'this is the deployment stage'
            }
        }
    }
}
