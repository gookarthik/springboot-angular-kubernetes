$ cd /home/ubuntu/test/springboot-angular-kubernetes

$ mvn package -Dmaven.test.skip=true
$ docker build -t gookarthik/angular-spring-mysql:spring .


$ docker images
$ docker tag 791eea6a7afd gookarthik/angular-spring-mysql:spring

$ docker push gookarthik/angular-spring-mysql:spring

$ cd /home/ubuntu/karthik-use/test/springboot-angular-kubernetes

$ kubectl apply -f kubernetes/
