Bootstrap
```
import { BrowserModule } from '@angular/core';
import { createCustomElement } from '@angular/elements';

@NgModule({
    imports: [BrowserModule],
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
