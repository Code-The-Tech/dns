# CodetheTech DNS



## Adding a subdomain

1. [Create a fork](https://docs.github.com/en/free-pro-team@latest/github/getting-started-with-github/fork-a-repo) of this repository.
2. In your fork open the [codethetech.tech](./codethetech.tech) file and add the following alphabetically based off the subdomain name:

```yaml
SUBDOMAIN_NAME:
  - ttl: 1
    type: CNAME
    value: Github or Vercel link.
```

3. Replace `SUBDOMAIN_NAME` with the name of the sub-domain. So if the name was `hello` then the subdomain would be `hello.codethetech.tech`.
4. Replace `Github or Vercel link` with the Github link or Vercel cname link of the website you want the subdomain to go. If you are using an IP address change `type: CNAME` to `type: A`. Remember to leave that `.` at the end!
5. Commit your changes and [create the PR](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request-from-a-fork)!

That's it! Someone with contributor access to the repo will then review your PR.

## Limitations

`codethetech.xxx` subdomains are only available for all clubs and projects related to CodetheTech.

When adding a site hosted on ▲ Vercel, you will need to verifiy the domain by adding a CNAME or TXT record.

<img width="787" alt="image" src="https://github.com/Code-The-Tech/dns/assets/85977707/7a1c770d-a6b3-4437-8569-775f4a073148">

Add the value to the [codethetech.tech](./codethetech.tech)
file as shown below:

```yaml
_vercel:
  ttl: 1
  type: CNAME
  values:
    - cname.vercel-dns.com.
 ```
