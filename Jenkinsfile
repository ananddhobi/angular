pipeline {
    agent { label 'anand' }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
              sh 'cp -r /usr/lib/node_modules/@angular/cli/node_modules /home/user/jenkinnode-1/workspace/angular-pipeline2'
              sh 'pm2 start "ng serve" --name angular-pipeline2'
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
