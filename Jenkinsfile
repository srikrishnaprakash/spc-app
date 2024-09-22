pipeline {
    agent any
    stages {
        stage ("Cloning Currency converter Application") {
            steps {
                git(
        			url: "https://github.com/srikrishnaprakash/spc-app.git",
        			credentialsId: "",
        			branch: "main"
		        )
            }
            
        }
        stage ("Packaging the application using maven") {
            steps {
               bat "mvn package -DskipTests"
            }
        }
    }
}