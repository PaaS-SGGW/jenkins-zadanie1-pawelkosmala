pipeline {
    agent any
    stages {
        stage('Heroku') {
            steps {
				bat "heroku git:remote -a pawelkosmala"
				bat "git push heroku HEAD:master"
            }
        }
    }
}
