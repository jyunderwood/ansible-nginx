# Ansible NGINX

Installs NGINX with via the offical apt repo for Debian-based systems.

This role does not do anything else, such as configure firewall options. It only installs NGINX.

## Usage

Requires `sudo` or root access.

```yaml
  hosts: all
  sudo: yes

  roles:
    - jyunderwood.nginx
```

## Variables

`nginx_remove_default_server_confs` (default: no) Will delete the `default` and `example_ssl` server config files.
`nginx_replace_default_http_conf` (default: no) Will replace the default `nginx.conf` config file.

## License

This Ansible role is licensed under the MIT License.

Copyright (c) 2014 Jonathan Underwood

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
