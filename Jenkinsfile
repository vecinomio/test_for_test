pipeline {
    agent none

    stages {

        stage ('Do on master jenkins') {
            agent {
                label 'master'
            }
                steps {
                    echo 'Testing on master'
                    sh 'echo $USER'
                    sh 'hostname'
                }
        }
        stage ('Do on cnt7') {
            agent {
                label 'cnt7'
            }
                steps {
                    echo 'Trying some tests on cnt7'
                    //sh 'vagrant provision --provision-with'
                    sh 'echo $USER'
                    sh 'hostname'
                }
        }
        stage ('Deploy') {
            steps {
                echo 'Deploy something'
            }
        }

    }

}
