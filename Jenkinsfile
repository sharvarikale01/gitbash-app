pipeline {
 
     agent{
                 label{
                         label "slave-1"
                         customWorkspace "/mnt/pipeline"

}
}

stages{
stage("stage-1"){
steps{
sh "yum install httpd -y"
sh "service httpd start"
sh"sudo cp -r index.html     /var/www/html"
sh "sudo chmod -R 777 /var/www/html/index.html"


}
}



}
