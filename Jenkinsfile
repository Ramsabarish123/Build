pipeline{
	agent {
		label 'master'
	}
	parameters {
		text(name: 'MANIFESTS', defaultValue: '<?xml version="1.0" encoding="UTF-8"?><manifest>  <remote name="origin" fetch="ssh://git@sdll9202.labs.teradata.com/source-code" />  <default revision="16.60DRS_SLES11.3_experimental" remote="origin" sync-j="4" />  <project name="tdbms" path="vob/dbsv2" />  <project name="tdbms" path="vob/dbsv2" />  <project name="tvsa" path="vob/tvsa" />  <project name="opnpde" path="vob/opnpde" />  <project name="gateway" path="vob/gateway" />  <project name="tdgss" path="vob/tdgss" />  <project name="suselinux-x8664" path="vob/suselinux-x8664" />  <project name="redhatlinux-x8664" path="vob/redhatlinux-x8664" />  <project name="icu" path="vob/icu" />  <project name="geospatial" path="vob/geospatial" />  <project name="java" path="vob/java" />  <project name="opnsrc" path="vob/opnsrc" />  <project name="tdv" path="vob/tdv" />  <project name="other" path="vob/" />  </manifest> ')
                string(defaultValue: "opnpde,tvsa,tdbms,tdgss,gateway", name: 'CHANGED_PROJECTS')
	        string(defaultValue: "16.50.00.00_CIW_83_S11SP3", name: 'PACKAGE_VERSIONS') 
		string(defaultValue: "SLES11.3", name: 'YUM_REPO') 
	}
	stages {
		stage('Build') {
			 sh 'echo ${MANIFESTS}'
		 }
	}
}
