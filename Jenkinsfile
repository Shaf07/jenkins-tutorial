pipeline{
        agent any
        stages{
             stage('clone sh repo'){
                steps{
                    git branch: 'main', url: 'https://github.com/Shaf07/jenkins-tut-2.git'
                        }
                }
            stage('run script'){
                steps{
                    sh 'myscript'
                }
            }
            stage('output'){
                steps{
                    archiveArtifacts artifacts: 'output', followSymlinks: false
                }
            }
        }
}
