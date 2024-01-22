Setup:
- run ```npm i && npm start``` for both client and server side to start the app

- For the following error in client side:  opensslErrorStack: [ 'error:03000086:digital envelope routines::initialization error' ],
  library: 'digital envelope routines',
  reason: 'unsupported',
  code: 'ERR_OSSL_EVP_UNSUPPORTED'

}
Please Try:

Linux and macOS (Windows Git Bash)-
export NODE_OPTIONS=--openssl-legacy-provider


Windows command prompt-
set NODE_OPTIONS=--openssl-legacy-provider


Windows PowerShell-
$env:NODE_OPTIONS = "--openssl-legacy-provider"



