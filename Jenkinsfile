pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install mydockerrepo1 petclinic  --set image.repository=registry.hub.docker.com/machendra1234/mydockerrepo1 --set image.tag=2'
              			
            }           
        }
    }
}
