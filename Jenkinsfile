pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install ankitasthana-app Helm_Deployment --set image.repository=registry.hub.docker.com/anasthan/petclinic --set image.tag=1'
              			
            }           
        }
    }
}
