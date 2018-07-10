# HostListener

```
@Component({
    selector: 'danger-button',
    template: `...`
})
export class DangerButtonComponent {
    constructor(el: ElementRef) {
        el.nativeElement // Angular Element
    }

    @HostListener('click')
    onHostClick($event) {}
}
```
