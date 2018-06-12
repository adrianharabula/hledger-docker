## Usage instructions
Run the webserver with
```
docker run -d -p 5000:5000 --restart=always --name=hledger adrianharabula/hledger hledger-web --serve --host=0.0.0.0 --port=5000
```
The journal file used is `/root/.hledger-journal`.

After running container, access web interface at http://localhost:5000

Additionally run hledger commands with:
```
docker exec hledger hledger balance
```
