Ansible Compile Website
=======================

Simple Ansible role that recursively wget some website in order to make it completely fill it's cache.

This step can take a while to run because it does crawl all the website.

All the command's output is deleted afterwards.


Example usage
-------------

```yaml
- role: compile-website
  compile_website_scheme: "https" # http or https
  compile_website_host: "savoirfairelinux.com" # the hostname / domain name
  compile_website_basepath: "/" # the base where to crawl
  compile_website_sleep: 1 # number of seconds to sleep between each requests
```
