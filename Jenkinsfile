#
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
    post {
        always {
        	cleanWs(cleanWhenNotBuilt: false,
            	deleteDirs: true,
            	disableDeferredWipeout: true,
            	notFailBuild: true,
            	patterns: [[pattern: '.gitignore', type: 'INCLUDE'],
            	[pattern: '.propsfile', type: 'EXCLUDE']])
     	}
   }
}

