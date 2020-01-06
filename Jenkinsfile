node {
	
	stage ('Checkout'){
		git url: "https://github.com/Pradeepv30/nodejs-runtime-agent.git"
	}
	stages ('snyk scan'){
		snykSecurity snykInstallation: 'Snyk-latest', snykTokenId: 'snyk-token', targetFile: 'package.json'
	}
}