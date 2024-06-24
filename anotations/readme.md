instalar no ubuntu
sudo apt-get install libssl-dev

necessario para rodar "sqlx migrate add -r init"
cargo install sqlx-cli


run:
		cargo run
watcher:
		cargo watch -q -c -w src/ -x run
migration_up:
		sqlx migrate run
migration_down:
		sqlx migrate revert