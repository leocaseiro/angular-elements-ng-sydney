## Attributes and Properties

```
class HelloWorld extends HTMLElement {
    name: string;

    static get() observedAttributes = ["name"];

    attributeChangedCallback(key, oldValue, newValue) {
        if (oldValue !== newValue) {
            this.name = newValue;
        }
    }

    set name(value) {}
    get name() {}
}
```

<pre class="fragment">
<code data-trim>
    <hello-world name="Leo Caseiro"></hello-world>
</code>
</pre>

<p class="fragment">Similar: Angular @Input() and @HostBinding()</p>
<p class="fragment">Similar: React props</p>
