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
                    BRANCH_NAME= 'dev' || BRANCH_NAME= 'master'
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