1/ Thực thi câu lệnh SQL

dattran@M-J40PFC4GC4 techmaster-obo-web % docker run -itd -p 3306:3306 -e MYSQL_ROOT_PASSWORD=123 -e MYSQL_DATABASE=obo -v /Users/dattran/techmaster-obo-web/obo.sql:/docker-entrypoint-initdb.d/init.sql --name mysql -d mysql

2. Export cac bien moi truong

export DB_HOST="localhost"
export DB_PORT="3306"
export DB_NAME="obo"
export DB_USER="root"
export DB_PASSWORD="123"

3. Chay ung dung JAVA
mvn spring-boot:run


Đăng nhập bằng user admin



4/ Đóng gói ứng dụng Java

#mvn install


5. Build Image

dattran@M-J40PFC4GC4 techmaster-obo-web % docker build . -t dangkiabcd/k8s-tech-labfinal:1.0





https://hub.docker.com/r/dangkiabcd/k8s-tech-labfinal
