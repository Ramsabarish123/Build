pipeline{
	agent {
		label 'master'
	}
	parameters {
		text(name: 'MANIFESTS', defaultValue: 'hello')
                string(defaultValue: "hi", name: 'CHANGED_PROJECTS')
	        string(defaultValue: "16.50.00.00_CIW_83_S11SP3", name: 'PACKAGE_VERSIONS') 
		string(defaultValue: "SLES11.3", name: 'YUM_REPO') 
	}
	stages {
		stage('Build') {
			 steps {
                		echo "flag: ${params.userFlag}"
            		}
		 }
	}
}
