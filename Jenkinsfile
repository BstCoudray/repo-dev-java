node {
    def app
     stage('Clone-checkout'){
        checkout scm
     }
     stage('Build image'){
        app = docker.build("dev-java/nginx")
     }
     stage ('Test'){
        withDockerContainer("dev-java/nginx"){ 
            sh "echo 'bonjour ici java à partir de nginx'" 
            }
            }
}
