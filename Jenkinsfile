pipeline {
  agent {
    docker {image 'ubuntu/apache2'}
  }
  stages {
    stage('Build') {
      steps {
         sh '''docker run -it --name my-apache-server -p 8081:80 -v "$PWD":/var/www/html/index.html'''
}
}
}
}
