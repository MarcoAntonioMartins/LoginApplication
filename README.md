# LoginApplication
Sistema base de login para outros projetos

- Comando para iniciar o Projeto:
    ```
    bundler install
    npm install

    rake db:create

    foreman start
    ```

Linha de tempo dos comandos de Criação:

- [Create Project](https://github.com/MarcoAntonioMartins/LoginApplication/commit/9b3239949c398abcb93df4edb30be64d23f16e1d)
    ```
    rails new LoginApplication -c bootstrap
    rake db:create
    ```
    
- [Config Rspec](https://github.com/MarcoAntonioMartins/LoginApplication/pull/3)
    ```
    rails generate rspec:install
    ```

- [Install Devise(Login)](https://github.com/MarcoAntonioMartins/LoginApplication/pull/3)

    Nesse passo foi nescessario instalar o foreman
    ```
    gem install foreman
    npm install -g yarn
    npm install
    ```
    
    add gem 'devise' in Gemfile
    ```
    bundle install
    rails generate devise:install
    ```

    Gerar controllers
    ```
    rails generate controller home index
    ```

    instalar simple_form
    ```
    rails generate simple_form:install --bootstrap
    ```

    Gerar devise user
    ```
    rails generate devise user
    bundle exec rake db:migrate RAILS_ENV=development
    ```

    Gerar telas do devise
    ```
    rails generate devise:views
    ```
