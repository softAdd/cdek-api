# CDEK API For JavaScript

# Important! NOT READY YET!!!1
## DO NOT USE ANYWARE
### IF YOU GOT AN ERROR I GUESS CDEK IS DOWN AGAIN ...

 ### Importing library

You can import the generated bundle to use the whole library generated by this starter:


### Install

```bash
npm install cdek-api
```

### Usage

```javascript
import Cdek from 'cdek-api'

const { CDEK_ACCOUNT, CDEK_SECURE_PASSWORD } = process.env

const cdek = new CdekApi(CDEK_ACCOUNT, CDEK_SECURE_PASSWORD)

Promise.resovle().then(async () => {
  const response = await cdek.statusReport({
    _DispatchNumber: '1094801704'
  })
  console.log(response.Order)
}).catch(error => console.error(error))
```
