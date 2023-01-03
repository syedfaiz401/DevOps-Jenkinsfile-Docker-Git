pipeline {
    agent any

    stages {
        stage('Build&Deploy') {
            steps {
             // Get SHA1 of current commit
                
              }
             // remove previous containers 
             // BUILD the Docker image
             sh "sudo docker build -t image-name:${commit_id} ."
             // SDEPLOYMENT:  Running docker container as my application   
             sh "sudo docker run -d -p 81:80 --name mycontainer image-name:${commit_id}" 
            }
        }
    }    
}
