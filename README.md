#HTTP-TLS
---------------------------------------------------------------------------
node jsfile [METHOD] [TARGET] [PROXIES] [DURATION] [RPC] [THREADS]
---------------------------------------------------------------------------
node http1.js GET "https://target.com" http.txt 120 64 1
node http2.js GET "https://target.com" http.txt 120 64 1
---------------------------------------------------------------------------
node jsfile [TARGET] [DURATION] [THREADS] [RPC] [PROXIES]
---------------------------------------------------------------------------
node tls.js "https://target.com" 120 1 RPC http.txt
---------------------------------------------------------------------------
