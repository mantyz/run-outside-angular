# @RunOutsideAngular

An **Angular** class decorator that wrap all class methods on ngZone.runOutsideAngular(). Add method names which should be excluded in config.

```js
import RunOutsideAngular from 'run-outside-angular'

@RunOutsideAngular({
    exclude: ['yo']
})
@Component({...})
export class ExampleComponent {
    yo() {
        // will be runned in Angular Zone
    }

    hoho() {
        // will be runned out Angular Zone
    }
}
```
