pipeline{
        agent any
        stages{
            stage('Make Directory'){
                steps{
                    library identifier: 'docker', retriever: modernSCM([$class: 'GitSCMSource', credentialsId: '', remote: 'https://gitlab.com/qacdevops/chaperootodo_client', traits: [gitBranchDiscovery()]])
                }
            }
            stage('Make Files'){
                steps{
                    sh "touch ~/jenkins-tutorial-test/file11 ~/jenkins-tutorial-test/file21"
                }
            }
        }
}
