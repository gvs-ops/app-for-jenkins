pipeline {
    environment{
        OWNER_NAME   = "Gonchar Vladislav"
        PROJECT_NAME = "Avos and Fedos"
    }
    
    agent any

    stages {
        stage('1-Build') {
            steps {
                echo 'Start of stage Build'
                echo 'Building'
                echo 'End of stage Build'
            }
        }
    stage('2-Test') {
            steps {
                echo 'Start of stage Test'
                echo 'Testing'
                sh   '''
                ls -la
                echo "Hellow ${OWNER_NAME}"
                echo "The project name ${PROJECT_NAME}"
                '''
                echo 'End of stage Test'
            }
        }
    stage('3-Deploy') {
            steps {
                echo 'Start of stage Deploy'
                echo 'Deploying'
                sh '''
                    echo "Line1"
                    echo "Line2"
                '''
                echo 'End of stage Deploy'
            }
        }
    }
}
