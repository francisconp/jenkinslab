
pipeline {
    agent any
    stages {
        stage('Deploy') {
          input {
            message "Which Version?"
            ok "Deploy"
            parameters { booleanParam(name: 'APP_VERSION', defaultValue: true, description: 'Namespace')
                        booleanParam(name: 'APP_VERSION', defaultValue: true, description: 'Deployment')
                        booleanParam(name: 'APP_VERSION', defaultValue: true, description: 'ConfigMaps')
                        booleanParam(name: 'APP_VERSION', defaultValue: true, description: 'Services')
                        booleanParam(name: 'APP_VERSION', defaultValue: true, description: 'Ingress') }
          }
          steps {
            echo "Deploying ${APP_VERSION}."
          }
        }
    }
}
