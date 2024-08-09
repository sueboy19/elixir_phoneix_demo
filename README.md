# elixir_phoneix_demo
1. git clone
2. ```
   docker compose up --build
   ```
3. http://localhost:4000

# Steps for Demo
1. Mac Install mix  [https://elixir-lang.org/install.html[Uploading config.exs…]()
](https://elixir-lang.org/install.html)
   ```
   brew install elixir
   ```
2. Install Phoenix [https://hexdocs.pm/phoenix/installation.html#phoenix](https://hexdocs.pm/phoenix/installation.html#phoenix)
   ```
   mix archive.install hex phx_new
   ```
4. make Relase continer (https://hexdocs.pm/phoenix/releases.html#containers)[https://hexdocs.pm/phoenix/releases.html#containers]
   ```
   mix phx.gen.secret # keep SECRET
   ```
   Replace docker-compose.yml SECRET_KEY_BASE、DATABASE_URL
   ```
   mix phx.gen.release --docker
   ```
6. Big problems is db and migrate, maybe need mix ecto.migrate... so... just use elixir_phoneix_demo
