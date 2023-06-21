pipeline{

    agent any
    environment{
        NEW_VERSION = '1.3.0'
    }
    stages{
        stage("build"){
            steps{
                echo "build"
                echo "build ver ${NEW_VERSION}"
            }
        }
        stage("test"){
            when{
                expression{
                    BRANCH_NAME= 'dev' 
                }
            }
            steps{
                echo "test"
            }
        }
        stage("deploy"){
            steps{
                echo "deploy"
            }
        }
    }
}