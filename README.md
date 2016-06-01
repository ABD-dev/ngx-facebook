[![npm](https://img.shields.io/npm/l/express.svg)](https://www.npmjs.com/package/ng2-facebook-sdk)

[![NPM](https://nodei.co/npm/ionic-native.png?stars&downloads)](https://nodei.co/npm/ng2-facebook-sdk/)


# Angular2 Facebook SDK

**NOTE**: This is work under progress. Watch this repo to be updated.

### Installation
Install via NPM:
```
npm i --save-dev ng2-facebook-sdk
```

Install via Bower:
```
bower install ng2-facebook-sdk
```

### Example Usage
```typescript
import {FacebookService, FacebookLoginResponse} from 'ng2-facebook-sdk/dist';

@Component({
  templateUrl: '/path/to/template.html',
  providers: [FacebookService]
})
export class MyComponent {
  constructor(private fb: FacebookService) { }

  someFunction(): void {
    this.fb.login().then(
      (response: FacebookLoginResponse) => console.log(response),
      (error: any) => console.error(error)
    );
  }
}
```
