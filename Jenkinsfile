pipeline {

    agent any

    stages {

        stage('Echoing') {

            steps {
              // Echo block
                sh '''
                echo "hi Lavanya"
                echo "Learning groovy"
                # shell comment
                pwd
                echo "inside Echoing block"
                '''
                    }

                         } // echo blockclosure

         stage('Run script') {

            steps {

               sh '''
               sh ./run.sh
               '''
                    }

                            } // Run blockclosure

        }  // Closes Stage block
        post {
            always {
                archiveArtifacts # '*.zip'
                   }
             }
    }
      
