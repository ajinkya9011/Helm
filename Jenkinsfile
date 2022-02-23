pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install ajinkya-app petclinic  --set image.repository=acr8983.azurecr.io/ajinkya --set image.tag=2'
              			
            }           
        }
    }
}
