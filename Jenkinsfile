pipeline{

    agent any

    stages{
        stage("build"){
            steps{
                echo "build"
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