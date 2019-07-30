# ELK Stack

```
$ cd deployment
$ ansible-playbook --inventory=<HOST>, --user=<USER> --private-key=<SSH_PRIVATE_KEY_PATH> site.yml
```

2. Add nginx `proxy_pass` on a HTTP bastion host

```
proxy_pass http://INTERNAL_GCP_DNS_NAME;
```

3. Add a CNAME DNS record corresponding with the nginx configuration.
4. Configure HTTPs with certbot
