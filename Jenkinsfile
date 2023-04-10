pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm  --install petclininc-app /var/lib/jenkins/workspace/petclinic-deployment  --set image.repository=registry.hub.docker.com/machendra1234/mydockerrepo1 --set image.tag=1'
              			
            }           
        }
    }
}
