## CustomEvent()

```
class DangerButton extends HTMLButtonElement {
    onClick() {
        this.dispatchEvent(
            new CustomEvent("show-validation",
                { form: isValid }
            )
        );
    }
}
```

<pre class="fragment">
<code data-trim>
    const dangerBtn = document.querySelector('danger-button');
</code>
</pre>

<pre class="fragment">
<code data-trim>
    dangerBtn.addEventListener("show-validation", event => { ... });
</code>
</pre>

<p class="fragment">Similar: @Output()</p>
