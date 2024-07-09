pipeline {
    agent any

    stages {
        stage('test') {
            steps {
                script {
                    sh '''
                        if [ "$(sudo docker ps --filter "name=mongoDB-Saif" --filter "status=running" -q)" ] || [ "$(sudo docker ps --filter "name=mongoExpress-Saif" --filter "status=running" -q)" ]; then
                            echo "Already Running!!!"
                        else
                            echo "Runing........."
                            sudo  docker-compose -f dockerComposeFile.yaml up -d
                        fi
                    '''
                }
            }
        }
    }
}

