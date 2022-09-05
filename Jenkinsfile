pipeline{
        agent any
        stages{
            stage('Make Directory'){
                steps{
                        sh "curl https://get.docker.com | sudo bash"
                }
            }
            stage('Make Files'){
                steps{
                    sh "touch ~/jenkins-tutorial-test/file11 ~/jenkins-tutorial-test/file21"
                }
            }
        }
}
