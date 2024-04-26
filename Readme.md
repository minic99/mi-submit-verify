# Submit Verifier

Submit Verifier is a utility for verifying submission formats. It provides methods to validate various formats such as email, phone number, date, URL, ID card, IP address, and username.

## Installation

You can install Submit Verifier via npm:

```bash
npm install mi-submit-verifier
```

## Useage
```js
const SubmitVerifier = require('submit-verifier');

// Create an instance of SubmitVerifier
const verifier = SubmitVerifier.create();

// Example submission data
const submission = {
  title: 'Example Submission',
  description: 'This is an example submission.',
  author: 'John Doe',
  email: 'john.doe@example.com',
  age: 25,
  phone: '12345678901',
  date: '2022-10-15',
  url: 'https://example.com',
  idCard: '123456789012345678',
  ipAddress: '192.168.1.1',
  username: 'johndoe123'
};

// Verify the submission format
const isValidSubmission = verifier.verifySubmission(submission);
console.log('Is valid submission:', isValidSubmission);
```