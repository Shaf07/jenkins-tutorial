pipeline{
        agent any
        stages{
             stage('clone sh repo'){
                steps{
                    git branch: 'main', url: 'https://github.com/Shaf07/jenkins-tut-2'
                        }
                }
            stage('run script'){
                steps{
                        sh 'sh ./myscript.sh'
                }
            }
            stage('output'){
                steps{
                    archiveArtifacts artifacts: 'output', followSymlinks: false
                }
            }
        }
}
