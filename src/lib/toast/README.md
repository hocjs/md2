# Md2Toast
Toast is a service, which show notifications in the view.

### Methods

| Name | Description |
| --- | --- |
| `toast(message: string)`/`show(message: string)` | Creates and show a simple toast noticiation. |


### Examples
A Toast would have the following script.
```ts

import {Md2Toast} from 'md2/toast/toast';

@Component({
  selector: "..."
})

export class ... {
    
  ...
  constructor(private toast: Md2Toast) { }
  toastMe() {
    this.toast.show('Toast message...');

    ---  or  ---

    this.toast.show({ message: 'Toast message...', hideDelay: 1000 });
  }

  ...

}
 ```