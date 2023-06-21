CODE_CHANGES = getGitChanges()
pipeline{

    agent any

    stages{
        stage("build"){
            when{
                expression{
                    BRANCH_NAME= 'dev' && CODE_CHANGES= true
                }
            }
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