pipeline{
    agent any
    stages{
        stage('clone'){
            steps{
                git 'https://github.com/Sharathkumarbm/demo1.git'
            }
        }
        stage('clean'){
            steps{
                sh 'mvn clean'
            }
        }
        stage('build'){
            steps{
                sh 'mvn install'
            }
        }
	    stage ('build image') {
		    steps {
			    sh 'docker build .'
    }
}
    }
}
