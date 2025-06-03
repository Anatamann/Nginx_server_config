# Nginx Server Setup ⚙
Nginx server config file setup example.
## HTTPS Redirection 🔧:
- Catches all HTTP traffic (port 80)
- 301 permanent redirect to HTTPS
- Includes HSTS header even in redirect responses

## Security Headers 🔏:
- Strict-Transport-Security enforces HTTPS
- X-Content-Type-Options prevents MIME sniffing
- X-Frame-Options protects against clickjacking
- Content-Security-Policy mitigates XSS risks
- Referrer-Policy controls referrer information

## Load Balancing ⚖:
- least_conn load balancing method
- Backend server pool with keepalive connections
- Proper header forwarding for origin servers
- Connection/timeout optimizations

