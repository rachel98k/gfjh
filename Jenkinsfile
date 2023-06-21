pipeline{

    agent any
    // parameters{
    //     choice(name: 'VERSION', choices:['1.1.0','1.2.0','1.3.0'],description:'')
    //     booleanParam(name: 'executeTests', defaultValue: true,description:'')
    // }
    // tools{
    //     maven 'Maven'
    // }
    // environment{
    //     NEW_VERSION = '1.3.0'
    //     SERVER_CREDENTIALS = credentials('')
    // }
    stages{
        stage("build"){
            steps{
                echo "build"
                // echo "build ver ${NEW_VERSION}"
            }
        }
        stage("test"){
            // when{
            //     expression{
            //         params.executeTests
            //     }
            // }
            steps{
                ech params.executeTests
            }
        }
        stage("deploy"){
            steps{
                echo "deploy"
            }
        }
    }
    post{
        always{
            echo "alw"
        }
        failure{
            echo "ffff"
        }
    }
}