pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm  upgrade --install petclininc-app petclinic  --set image.repository=registry.hub.docker.com/kittu64/petclinic --set image.tag=latest'
              			
            }           
        }
    }
}
