#!groovy
pipeline {
    agent any
    triggers {
        pollSCM('H/3 * * * 1-5')
    }
    environment {
        MAIN_DIR = ''
    }
    stages {
        stage('Develop Branch <server dev>') {
            when {
                branch 'develop'
            }
            steps {
                ansiColor('xterm') {
                    echo '<<< start develop >>>'
                }
            }
        }
        /*stage('Master Branch <server prd>') {
        when {
            branch 'master'
        }
        steps {
            ansiColor('xterm') {
                echo '<<< start develop >>>'
            }
        }
    }*/
    }
}