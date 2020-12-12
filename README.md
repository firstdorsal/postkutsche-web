**This is a mirror of [git.y.gy/firstdorsal/postkutsche-web](https://git.y.gy/firstdorsal/postkutsche-web)**
# postkutsche-web
<img draggable="none" src="https://git.y.gy/firstdorsal/postkutsche-web/-/raw/master/logo.jpg" style="float:left; margin-right:10px;" height="100"> 

## Postkutsche is a module that combines PowerDns and Mailcow to create a mail domain with all required entries on both services in a single command. This is the same module packed in a single html file ready to be executed directly in your browser without downloading anything else!

## The TLSA record creation is **NOT** supported in the browser as it requires openssl to be executed.

# Install
Download the index.html from this repository: [here](https://git.y.gy/firstdorsal/postkutsche-web/-/raw/master/index.html?inline=false) and open it in the browser.

# Basic use
## With the dev console
1. Press F12 or ctrl/strg + shift + i to open the developer tools and navigate to the console.

1.1 If the console is not directly visible press 'ESC' to open it

2. Create a Postkutsche client
```js
let pk=new Postkutsche({mailcow:{url:"https://mail.example.com",apikey:"yourMailcowApiKey"},powerdns:{url:"https://example.com/api/v1/servers/localhost",apikey:"yourPdnsApiKey"}});

await pk.openpgpHash('your.local.email.name');
```
## By adding to the file
Go to the bottom of the index.html and add your functions.

# Use the powerdns-api or the mailcow-api without postkutsche
```js
let mailcowClient=new MailcowApiClient('https://mail.example.com','yourMailcowApiKey');

```
OR
```js
let powerdnsClient=new PowerdnsClient('https://example.com/api/v1/servers/localhost','yourPdnsApiKey');

```
# Check out the documenations of the modules

## postkutsche
[NPM](https://www.npmjs.com/package/postkutsche)

[Documentation](https://doc.y.gy/postkutsche/)

[Code](https://git.y.gy/firstdorsal/postkutsche)

### powerdns-api
[NPM](https://www.npmjs.com/package/@firstdorsal/powerdns-api)

[Documentation](https://doc.y.gy/powerdns-api/)

[Code](https://git.y.gy/firstdorsal/powerdns-api)

### mailcow-api
[NPM](https://www.npmjs.com/package/mailcow-api)

[Documentation](https://doc.y.gy/mailcow-api/)

[Code](https://git.y.gy/firstdorsal/mailcow-api)

# Need help or missing a feature?
Feel free to contact me via [xl9jthv_7bvgakv9o9wg0jabn2ylm91xxrzzgt0e@y.gy](mailto:xl9jthv_7bvgakv9o9wg0jabn2ylm91xxrzzgt0e@y.gy) in english or german
