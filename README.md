# infra-challenge

**To run the project clone the git repo from the link and execute the command given below from the root directory where docker-composer.yaml file exist.**
```
# docker-compose up --build -d
```
Note: (if it shows error : strconv.Atoi: parsing "": invalid syntax or any network conflict error Please run the command below to removes the resources not associated with a container.
**# docker system prune** )

**To Access the Services Use those URLs from your Browser.**
```
http://localhost:3000/orders
```
```
http://localhost:4000/products
```
```
http://localhost:5000/users
```


**Use this command to terminate the project.**
```
# docker-compose down
```
