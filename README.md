# electron-local-key-value
 Local Store Key Value For Electron

 ## Install

 `npm install electron-local-key-value`

 ## Usage

 This package can use both main process and renderer process

`
const Store = require('../Store');
const storage = new Store({
    filename: 'app-config',
    default: {}
});

storage.set('KEY', 'value');

console.log(storage.get('KEY'));
// Result : 'value';

console.log(storage.get('KEY_NOT_FOUND'));
// Result : underfined;

store.commit(); // Save to file

`