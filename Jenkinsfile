node('nodejs') {
	stage('Checkout') {
		git branch: 'main',
			url: 'https://github.com/sashperso/do400-pipelines-control'
	}
	stage('Backend Test') {
		sh 'node ./backend/test.js'
	}
	stage('Frontend Test') {
		sh 'node ./frontend/test.js'
	}
}
