node {
    def app

    stage('Clone repository') {
        checkout scm
    }

    stage('Build image') {
        app = docker.build("getintodevops/hellonode")
    }
    stage('Run image'){
    dir("/Users/digicodeanuj/Desktop/AS/project")
        sh 'docker run -it -p 8000:8000 getintodevops/hellonode'
        }
    }
    //stage('Test image') {
     //   app.inside {
       //     sh 'echo "Tests passed"'
        //}
   // }
    //stage('Push image') {
      //  docker.withRegistry('https://registry.hub.docker.com', 'docker-hub-credentials') {
        //    app.push("${env.BUILD_NUMBER}")
          //  app.push("latest")
       // }
    //}
}
