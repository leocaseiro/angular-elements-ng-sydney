## Customize Existing HTML Element

```
class DangerButton extends HTMLButtonElement {}

customElements.define(
    "danger-button",
    DangerButton,
    { extends: "button" }
);
```
<pre class="fragment">
<code data-trim>
    <danger-button></danger-button>
</code>
</pre>

<p class="fragment">Similar: Angular Directive or React.createElement()</p>
