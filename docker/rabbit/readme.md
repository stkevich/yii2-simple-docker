# Admin user
* docker exec shop_rabbit rabbitmqctl add_user admin admin
* docker exec shop_rabbit rabbitmqctl set_user_tags admin administrator
* docker exec shop_rabbit rabbitmqctl set_permissions -p / admin ".*" ".*" ".*"
 
# Application user
* docker exec shop_rabbit rabbitmqctl add_user app apPas
* docker exec shop_rabbit rabbitmqctl set_permissions -p / app ".*" ".*" ".*"