pipeline {
    agent any

    parameters {
        booleanParam(defaultValue: false, description: "Enable service?", name: "myBoolean")
    }

    stages {
        stage("Demo"){
            steps {
                script{
                    if (param.myBoolean == false){
                        currentBuild.result = "SUCCESS"
                        return
                    }
                    else {
                           echo "booleanParam is set to =TRUE"
                    }
                }
                
            }
        }
    }   
}
