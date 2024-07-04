# intl-input
intl-input is the selector for ionic3 to select multiple countries phone number.
This module works with ionic 3 all version  only.

Installation
------------

`npm install --save intl-tel-ionic3`

Usage
-----
Import `IntlTelModule` into your app's required page module

``` typescript
import { IntlTelModule } from  'intl-tel-ionic3'

@NgModule({
  imports: [
    IntlTelModule
  ]
})
```
Then, use it in your component:

``` typescript
@Component({
  selector: 'app',
  template: `
    <intl-input [(ngModel)]="mobileno" [config]="config" (onEnter)="onEnterdata($event)" ></intl-input>
  `
})
export class AppComponent {
    //config is mandatory without that it won't show on the front end
 public config = {
    placeholder: 'Mobile no',
    labletext: 'Contact *',
    textalign: 'right',
    maximumlength: 10,
    disabled: false,
    icon:true,
    iconName:"call"
  }
}
```
## Documentation
As you can see in the code above, you will get the output from 'onEnterdata' function.


if you have any query please send us a email on sarojctc2010@gmail.com
