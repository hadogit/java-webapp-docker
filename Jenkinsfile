pipeline {
    agent any
	stages {
		stage('Building image') {
			steps{
				script {
				docker.build registry + ":$BUILD_NUMBER"
				}
			}
		}
		//stage('Test image') {
        /* Ideally, we would run a test framework against our image.
         * For this example, we're using a Volkswagen-type approach ;-) */

		//	app.inside {
		//		sh 'echo "Tests passed"'
		//	}
		//}
	}
}