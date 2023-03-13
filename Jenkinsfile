pipeline { 
    agent any 
    stages { 
        /*
     * The below executes the ls command, prints out Hello Jenkins Build stage and executes the creation of mylabdoc.txt
     */
        stage('Build'){ 
            steps { 
                sh "ls"
                echo 'Hello Jenkins Build stage'
                sh 'touch mylabdoc.txt'
            } 
        } 
        stage('Test'){ 
            steps { 
               sh "pwd" 
               echo 'Test stage'
               sh 'mv mylabdoc.txt mylabdoc2.txt'
            } 
        } 
         stage('Deploy'){ 
            steps { 
                sh "ls"
                echo 'Deploy Stage'
            } 
         }
    }
}
