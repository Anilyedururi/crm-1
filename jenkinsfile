pipeline {
    agent any
    stages{
        stage("maven build") {
            when {
                branch 'develop'
            }
            steps {
                echo "maven build.."
            }    
        }
        stage("sonar analysis") {
            when {
                branch 'develop'
            }
            steps {
                echo "sonar analysis.."
            }    
        }
        stage("vulnarability scanning") {
            when {
                branch 'develop'
            }
            steps {
                echo "vulnarability scanning"
            }    
        }
        stage("dev deploy") {
            when {
                branch 'develop'
            }
            steps {
                echo "dev deploy"
            }    
        }
        stage("test deploy") {
            when {
                branch 'test'
            }
            steps {
                echo "test deploy"
            }    
        }
        stage("prod deploy") {
            when {
                branch 'master'
            }
            steps {
                echo "prod deploy"
            }    
        }
    }
}
