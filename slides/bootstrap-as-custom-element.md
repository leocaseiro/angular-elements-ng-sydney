Bootstrap
```
import { BrowserModule } from '@angular/platform-browser';
import { createCustomElement } from '@angular/elements';

@NgModule({
    imports: [BrowserModule],
    declarations: [MyAngularElementComponent],
    entryComponents: [MyAngularElementComponent]
})
export class AppModule {
    constructor(private injector: Injector) {}

    ngDoBootstrap() {
        customElements.define("my-angular-element",
            createCustomElement(MyAngularElementComponent,
                { injector: this.injector }
            )
        );
    }
}
```
