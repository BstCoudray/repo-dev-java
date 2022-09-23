node {
    def app
     stage('Clone-checkout'){
        checkout scm
     }
     stage('Build image'){
        app = docker.build("dev-java/apache")
     }
     stage ('Test'){
        withDockerContainer("dev-java/apache"){ 
            sh "echo 'bonjour ici java'" 
            }
            }
}
