pipeline {

agent {

lable {
lable  "built-in"
}
}

stages{
stage('install-apache'){
steps{
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

