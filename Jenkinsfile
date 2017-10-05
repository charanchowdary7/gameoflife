node {
       stage 'Checkout'
       checkout scm
           
       stage 'Build'
       def app = docker.build gameoflife/our-app:${env.BUILD_NUMBER}"

       stage 'Test'
       app.inside {
            sh '/app/run_tests.sh'
           } 
       stage 'Publish'
       app.push 'latest'
      }

