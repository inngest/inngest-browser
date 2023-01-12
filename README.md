## Inngest Browser SDK

This is the Inngest SDK to send events from the browser. If you're looking for the Inngest JavaScript/TypeScript Node.js SDK check out that repo here: https://github.com/inngest/inngest-js

## Usage

Add the script via [unpkg](https://unpkg.com/):

```html
<script src="https://unpkg.com/@inngest/browser/inngest.min.js" />
```

Initialize your client with an Inngest event key and send your event:

```js
inngest.init("<replace-with-your-event-key>");
inngest.send({
  name: "your.event.name",
  data: {
    useful: "information",
  },
  user: {
    // optionally append user data
    email: "test@example.com",
  },
});
```

That's it - you're now sending events from the browser.

> ⚠️ - **NOTE** - You should add an allow list for your events in the Inngest Cloud dashboard so

## Development

```bash
yarn build
yarn np # to publish
```
