pipeline {
    agent none

    stages {

        stage ('Do on master jenkins') {
            agent {
                label 'master'
            }
                steps {
                    echo 'Testing on master'
                    sh 'cd /home/makienko_ig && sudo touch makienko.txt'
                }
        }
        stage ('Do on cnt7') {
            agent {
                label 'cnt7'
            }
                steps {
                    echo 'Trying some tests on cnt7'
                    //sh 'vagrant provision --provision-with'
                    sh 'cd /home/makienko_ig && sudo touch bumblbee.txt'
                }
        }
        stage ('Deploy') {
            steps {
                echo 'Deploy something'
            }
        }

    }

}
