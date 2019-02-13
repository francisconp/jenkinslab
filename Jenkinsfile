
pipeline {
    agent any
    stages {
        stage('Deploy') {
          input {
            message "Which Version?"
            ok "Deploy"
            parameters {
                choice(name: 'APP_VERSION', choices: "v1.1\nv1.2\nv1.3", description: 'What to deploy?')
            }
          }
          steps {
            echo "Deploying ${APP_VERSION}."
          }
        }
    }
}
