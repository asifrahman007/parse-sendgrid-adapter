# Parse Server Sendgrid Email Adapter

## Installation

```sh
npm install parse-sendgrid-adapter
```

## Usage

```javascript
const { ParseServer } = require('parse-server');
const sendGridAdapter = require('parse-sendgrid-adapter');

const config = {
  ...,
  emailAdapter: sendGridAdapter({
    apiKey: '', // sendgrid api key
    from: {email: 'myapp@example.com', name: 'My App'}, // from email address,
    passwordResetTemplate : '', // sendGrid template ID
    verificationEmailTemplate : '' // sendGrid template ID
  })
};

const parseServer = new ParseServer(config);
```
