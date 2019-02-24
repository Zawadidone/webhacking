# Information disclosure

- [ ] Backup files
- [ ] Leaking stackt-traces
- [ ] Comments
- [ ] Path disclosure
- [ ] Directory listing

### Recon
[Use reddit for recon purposes](https://gist.github.com/EdOverflow/4856db4db4075b76dd00385adcedfb49)


### Path disclosure
```gobuster -w {wordlist.txt} -s {status codes} -u {url}``` | Bruteforce directories use [Fuzzdb](https://github.com/fuzzdb-project/fuzzdb)

### Directory listing
[Traversal Directory](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/8209d32bafaa679793e5249ad7ac8cfae8f33011/Traversal%20directory)


### Dorks - [Tips](https://medium.com/@khaled.hassan/bugbountyprotip-collection-4a19e5b5b296)
Dork    | Description
--------|------------
https://github.com/search?q={company-name}&type=Users | Search for company users or projects using Github
https://www.google.com/?q=inurl:https://trello.com AND intext:password AND inurl:{company-name} | Search for passwords in public Trello boards
