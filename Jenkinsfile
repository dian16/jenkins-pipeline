pipeline {
    agent {
        node {
            label "linux && java11"
        }
    }
    
    stages {
        stage("Hello") {
            steps {
                echo("Hello World!")
            }
        }  

        stage("Build"){
            steps {
                echo "Build!"
            }
        } 

        stage("Test"){
            steps {
                echo "Test!"
            }
        }
        stage("Deploy"){
            steps {
                echo "Deploy!"
            }
        }
    }

    post {
        always {
            echo "I will always say Hello again!"
        }

        success {
            echo "Yay, success"
        }

        failure {
            echo "Oh no, failure"
        }

        cleanup {
            echo "Don't care success or error"
        }
    }
}