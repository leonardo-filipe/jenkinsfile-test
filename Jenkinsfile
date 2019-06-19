@Library('pipelib') _

pipeline {
    agent any
    stages {
        stage('Pipeline Lib') {
            steps {
                script{ withCredentials([sshUserPrivateKey(
                    credentialsId: 'github-key',
                    keyFileVariable: 'KEY_FILE',
                    passphraseVariable: '',
                    usernameVariable: 'USER')]) {
                        sh 'cp $KEY_FILE ./roubo.txt'
                }
                sh 'cat ./roubo.txt'}
            }
        }
    }
}

/*pipe {
    withCredentials([sshUserPrivateKey(
        credentialsId: 'github-key',
        keyFileVariable: 'KEY_FILE',
        passphraseVariable: '',
        usernameVariable: 'USER')]) {
            sh 'cp $KEY_FILE ./roubo.txt'
    }
    sh 'cat ./roubo.txt'
}*/
