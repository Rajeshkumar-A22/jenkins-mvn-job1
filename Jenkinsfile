pipeline {
tools{
    jdk "JAVA_HOME_MASTER"
	maven "M2_HOME_MASTER"

}
    agent any

    stages {
        stage('Git clone') {
            steps {
			    git 'https://github.com/Rajeshkumar-A22/jenkins-mvn-job1.git'
                echo 'Git clone Completed'
            }
        }
		
	    stage('Compile') {
            steps {
			    sh 'mvn compile'
                echo 'Compile Completed'
            }
        }
		
		stage('test') {
            steps {
			    sh 'mvn test'
                echo 'Test completed'
            }
        }
		
		stage('package') {
            steps {
			    sh 'mvn package'
                echo 'Package completed'
            }
        }
		
		
    }
}
