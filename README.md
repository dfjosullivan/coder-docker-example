mkdir -p ./nginx/certificates
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout ./nginx/certificates/selfsigned.key -out ./nginx/certificates/selfsigned.crt -subj "/CN=localhost"


openssl dhparam -out ./nginx/certificates/dhparam.pem 2048
