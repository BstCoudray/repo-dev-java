node {
    def app
     stage('Clone-checkout'){
        checkout scm
     }
     stage('Build image'){
        app = docker.build("dev-java/httpd")
     }
     stage ('Test'){
        withDockerContainer("dev-java/httpd"){ 
            sh "echo 'bonjour ici java'" 
            }
            }
}
