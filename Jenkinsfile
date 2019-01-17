pipeline {
    agent {
        label 'cnt7'
    }
    //triggers {
        //pollSCM '* * * * *'
    //}

    stages {
        //stage ('Checkout') {
            //steps {
                //echo 'Checkout....'
                //checkout([$class: 'GitSCM', branches: [[name: '*']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/vecinomio/test_for_test.git']]])
            //}
        //}

        stage ('Build') {
            steps {
                echo 'Building....'
            }
        }
        stage ('Tests') {
            steps {
                echo 'Trying some tests'
                //sh 'vagrant provision --provision-with'
            }
        }
        stage ('Deploy') {
            steps {
                echo 'Deploy something'
            }
        }

    }

}
