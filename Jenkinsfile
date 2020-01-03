node {
	
	stage ('Checkout'){
		git url: "https://github.com/Pradeepv30/nodejs-runtime-agent.git"
	}
	stages ('snyk scan'){
		tools {
			snyk 'Snyk-latest'
		}
		steps {
			snykInstallation: 'Snyk-latest',
			snykTokenId: 'snyk-token',
			targetFile: 'requirements.txt',
			failOnIssues: 'false'
		}
	}
}