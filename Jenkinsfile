//@Library('pipelib') _

pipeline {
    agent any
    stages {
        stage('Pipeline Lib') {
            steps {
                echo 'Print from main Jenkinsfile repo.'
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
