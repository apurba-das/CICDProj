pipeline {
    
    node ("Slave_Node_1") {
        stages {
            stage ("Compile") {
                steps {
                    sh "mvn compile"
                }
            }
        }
    }
    
    node ("Slave_Node_2") {
        stages {
            stage("unit test") {
                steps {
                    sh "mvn test"
                }
            }
        }
    }
    
}
