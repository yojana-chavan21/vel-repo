pipeline {

  agent {
    lable {
lable  "built-in"
      customWorkspace ('/data/pipeline')
}
}

stages{
stage('install-apache'){
steps{
  sh "yum install httpd -y"
}
}


stage('deploy-index'){
steps{
sh "cp -r index.html /var/www/html/index.html"
sh "chmod -R 777 /var/ww/html/index.html"
}
}

stage('restart-apache'){
steps{
sh "service httpd restart"
}
}
}
}

