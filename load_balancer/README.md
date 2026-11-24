# Load balancer

Adding redundancy to the web stack: two Nginx web servers behind an HAProxy load balancer.

| File | Description |
| ---- | ----------- |
| `0-custom_http_response_header` | Configures Nginx (same as web-01) and adds an `X-Served-By` header with the server's hostname |
| `1-install_load_balancer` | Installs HAProxy on lb-01 and spreads traffic to web-01 and web-02 with `roundrobin` |

## Servers
| Name | IP |
| ---- | -- |
| 7123-web-01 | 18.133.158.178 |
| 7123-web-02 | 3.9.132.43 |
| 7123-lb-01 | 3.10.227.167 |
