
pipeline {
    agent any
    stages {
        stage('Deploy') {
          input {
            message "Which Version?"
            ok "Deploy"
            parameters { booleanParam(name: 'APP_VERSION', defaultValue: true, description: 'Namespace') }
            parameters { booleanParam(name: 'APP_VERSION', defaultValue: true, description: 'Deployment') }
            parameters { booleanParam(name: 'APP_VERSION', defaultValue: true, description: 'ConfigMaps') }
            parameters { booleanParam(name: 'APP_VERSION', defaultValue: true, description: 'Services') }
            parameters { booleanParam(name: 'APP_VERSION', defaultValue: true, description: 'Ingress') }
          }
          steps {
            echo "Deploying ${APP_VERSION}."
          }
        }
    }
}
