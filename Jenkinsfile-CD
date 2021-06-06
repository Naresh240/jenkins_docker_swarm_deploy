pipeline {
    agent { label 'docker-swarm' }
    stages {
        stage ('scm') {
            steps {
                git branch: 'main', url: 'https://github.com/Naresh240/jenkins_docker_swarm_deploy.git'
            }
        }
        stage ('Deployment') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'docker_credentials', passwordVariable: 'password', usernameVariable: 'username')]) {
                    sh "docker login -u ${username} -p ${password}"
                }
                sh 'docker stack deploy --compose-file docker-stack.yml springboot'
            }
        }
    }
}
