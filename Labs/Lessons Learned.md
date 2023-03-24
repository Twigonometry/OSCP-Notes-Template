In this note I collected all the key things I learned on the labs - useful commands for obscure services, alternative ways to enumerate for niche or well-hidden files, common pitfalls and issues with specific services or techniques, and things I wished I'd known when stuck in a rabbit hole for hours.

These lessons can really be anything - the purpose of this note is to look back at what mistakes you made, and to have a resource to look at when you're in a rut.

I split the lessons into vague categories, with links to the machines that I learned them on. An example layout is below.

## Enumeration

### Nmap

- Use the `-v` flag to see ports as they appear - this lets you explore the attack surface quicker

### Windows

- On old versions, there are some alternatives to `whoami`:
	- `set`
	- `systeminfo`
	- `net user`
	- `echo %username%`
	- `echo %userprofile%`

## Password Cracking

- Use the `-n` flag when echoing hashes to a file to avoid a trailing newline (see [[Andy Index|Andy]])