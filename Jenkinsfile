pipeline{
	agent {
		label 'master'
	}
	parameters {
		text(name: 'MANIFESTS', defaultValue: '')
                string(defaultValue: "opnpde", name: 'CHANGED_PROJECTS')
	        string(defaultValue: "", name: 'PACKAGE_VERSIONS') 
		string(defaultValue: "", name: 'YUM_REPO') 
	}
	stages {
		stage('Build') {
			 steps {
                		sh 'echo "Hello World"'
               			 sh '''
                   		    echo "Multiline shell steps works too"
                		    ls -l
                		'''
            		}
		 }
	}
}
