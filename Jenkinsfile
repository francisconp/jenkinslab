
pipeline {
    agent any
    stages {
        stage('Deploy') {
          input {
            message "Which Version?"
            ok "Deploy"
            parameters { booleanParam(name: 'APP_VERSION', defaultValue: true, description: 'teste') }
          }
          steps {
            echo "Deploying ${APP_VERSION}."
          }
        }
    }
}
