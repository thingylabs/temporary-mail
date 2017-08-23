# temporary-mail

> Temporary mailboxes for end-to-end testing, QA testing and crawling

## Install

```
npm install temporary-mail
```

## Usage

```js
import TemporaryMail from 'temporary-mail'

const mail = new TemporaryMail()

// Get an new mail address
const address = await mail.getAddress()
console.log(`address`, address)

// Read all emails
const mails = await mail.getMails()
console.log(`mails`, mails)

// Wait till a specific email arrives
const testMail = await mail.pollTillSubject(/test/i)
console.log(`testMail`, testMail)
```

## Licence

MIT
