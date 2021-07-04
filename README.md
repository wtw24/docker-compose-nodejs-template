# docker-compose-nodejs-template

Install Vue CLI as root
~~~
docker-compose exec -u 0 node-cli npm install -g @vue/cli
~~~

Create hello-world vue app
~~~
docker-compose exec node-cli vue create hello-world
~~~

CLI alias:
~~~
alias npm='docker-compose run --rm node-cli npm'
~~~