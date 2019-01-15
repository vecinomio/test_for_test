pipeline {
    agent any
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
            }
        }
        stage ('Deploy') {
            steps {
                echo 'Deploy something'
            }
        }

    }

}
