pipeline{
    agent any
    stages{
        stage("pre-build"){
            steps{
                sh 'npm install'
                sh 'npm run build'
            }
        }
//         stage("build"){
//             docker.build("saifromdhane/nodeserver")
//             docker.withRegistry('https://registry.hub.docker.com', 'git') {            
//                 app.push("${env.BUILD_NUMBER}")            
//                 app.push("latest")        
//             }    
//         }
        stage("post-build"){
            steps{
                sh 'echo "build success"'
            }
        }
    }
}
