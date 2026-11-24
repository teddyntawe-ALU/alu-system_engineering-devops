# Web server

Configuring an Nginx web server on Ubuntu with Bash scripts that run without any human intervention.

| File | Description |
| ---- | ----------- |
| `0-transfer_file` | Transfers a file to a server's home directory with `scp` (strict host key checking disabled) |
| `1-install_nginx_web_server` | Installs Nginx on port 80; `/` returns a page containing `Holberton School` |
| `2-setup_a_domain_name` | The domain name pointing to web-01 |
| `3-redirection` | Adds a `301 Moved Permanently` redirection on `/redirect_me` |
| `4-not_found_page_404` | Adds a custom 404 page containing `Ceci n'est pas une page` |
| `5-design_a_beautiful_404_page.html` | A designed 404 page |

## Key concepts
- **Web server**: software that accepts HTTP requests and returns pages/files.
- **Parent and child processes**: Nginx runs a master (parent) process that reads the config and manages worker (child) processes that handle requests.
- **Main HTTP requests**: GET, POST, PUT, DELETE, HEAD.
- **DNS** (Domain Name System) translates domain names into IP addresses.
  - `A` maps a name to an IPv4 address, `CNAME` aliases a name to another name,
    `TXT` holds text, `MX` names the mail server.
