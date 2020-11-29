pipeline {
        stages {
            stage ("Compile") {
                steps {
                    node ("Slave_Node_1") {
                        sh "mvn compile"
                    }
                }
            }            
            stage("unit test") {
                steps {
                    node ("Slave_Node_2") {
                        sh "mvn test"
                    }
                }
            }
        }
}
