    pipeline {
        agent { label 'master' }

        stages {
            stage('Code Quality Analysis') {
                steps {
                    sh 'sonar-scanner -Dsonar.login="${stoken}"'
                }
            }
            stage('Build') {
                steps {
                    echo 'Building..'
                }
            }
            stage('Test') {
                steps {
                    echo 'Testing..'
                }
            }
            stage('Deploy') {
                steps {
                    echo 'Deploying....'
                }
            }
        }
    }
