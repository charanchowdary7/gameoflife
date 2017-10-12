node {
   stage 'Stage 1'
   		echo 'Hello World 1'

   stage 'Checkout scm' 
   		checkout scm
   
   stage 'Build'
         app = docker.build("charanchowdary7/hello")
}
