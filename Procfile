
worker: npm start
db: node . --db "link mongodb" --autocleartmp --restrict
pm2: npm install && npm i -g pm2 && pm2 start index.js && pm2 save && pm2 logs
web: npx pm2 start npm --node-args="--optimize_for_size --max_old_space_size=460" -- run db && npx pm2 logs
server: node . --server 
