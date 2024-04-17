node{
    git branch: 'main', url: 'https://github.com/maherdevops/simple-java-app.git'
    stages{
            stage('build'){
            try{
            sh'echo "build stage"'
            }
            catch(Exception e){
                sh'echo "exception found"'
                throw e
            }

        }
    stage('test'){
        if (env.BRANCH_NAME == "feat"){
            sh'echo "test stage"'

        }
        esle{
            sh'echo "skip test stage"'
        }
    }

    }

    
    
}