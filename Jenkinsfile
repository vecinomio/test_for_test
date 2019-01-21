pipeline {
    agent none

    stages {

        stage ('Start cnt7') {
            agent {
                label 'master'
            }
                steps {
                    echo 'Starting instance'
                    sh 'gcloud compute instances start cnt7 --zone=europe-west3-c'
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
        stage ('Stop cnt7') {
            agent {
                label 'master'
            }
                steps {
                    echo 'Starting instance'
                    sh 'gcloud compute instances stop cnt7 --zone=europe-west3-c'
                }
        }

    }

}
