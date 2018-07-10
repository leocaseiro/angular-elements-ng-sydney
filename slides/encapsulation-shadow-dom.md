##  Setup Native Encapsulation

```
@Component({
    selector: 'danger-button',
    template: `<slot></slot>`, // similar ng-content
    encapsulation: ViewEncapsulation.Native // wait ng7 and Ivy
})
export class DangerButtonComponent {}
```

Slots + Shadom DOM - Experimental
