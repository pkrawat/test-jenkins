pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
    post {
        success {
            emailext body: 'test mail',
	            subject: "SUCCESSFUL: Automation",
	            to: '${MAIL_TO}'
        }

    }
}
