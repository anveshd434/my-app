pipeline {
    agent any 
    stages {
        stage('clean=======') { 
            steps {
                //sh "rm -rf my-app"
                //sh "git clone https://github.com/anveshd434/my-app.git"
               // sh "cd /Users/anvesh/.jenkins/workspace/pipelinejob"
              // sh "/usr/local/Cellar/maven/3.8.5/bin/mvn clean -f my-app"
              sh "/usr/local/Cellar/maven/3.8.5/bin/mvn clean"
            }
        }
        stage('Test') { 
            steps {
               // sh "cd"
               //sh "/usr/local/Cellar/maven/3.8.5/bin/mvn test -f my-app/"
              sh "/usr/local/Cellar/maven/3.8.5/bin/mvn test"
            }
        }
        stage('Package=======') { 
            steps {
               // sh "cd "
              sh "/usr/local/Cellar/maven/3.8.5/bin/mvn package" 
              // sh "/usr/local/Cellar/maven/3.8.5/bin/mvn package -f my-app/"
               // sh "cd /Users/anvesh/.jenkins/workspace/pipelinejob/my-app"
               // sh "/usr/bin/java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App"
            }
        }
    }
}
