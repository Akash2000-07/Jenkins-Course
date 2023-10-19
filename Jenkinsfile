pipeline {
    agent any

    parameters {
        booleanParam(defaultValue: false, description: "Enable service?", name: "myBoolean")
    }

    stages {
        stage("Demo"){
            steps {
                script{
                    if (param.myBoolean == true){
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
