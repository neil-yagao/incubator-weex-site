---
title: Platform Differences with Web
type: wiki
group: Design
order: 1.4
version: 2.1
---

# Platform Differences with Web

Weex is a cross-platform solution and web platform is just one of many runtimes environment.Beside web platform, weex would also run smoothly under Android and iOS platform. The differences could be found in both features and implementing experience between Native and Web.

## Weex do not have DOM
DOM(Document Object Model),is the interface for HTML and XML which is original from Web. Weex is mainly designed for native platform and rendered components are native components rather than DOM Element.

### No DOM Operations
Since native environment is not supporting Web API, which means weex does not have Object like `Element` 、`Event` 、`File` and you could find the full list at [Web APIs on MDN](https://developer.mozilla.org/en-US/docs/Web/API).

### Limited Event Type

Weex is supporting binding event directly on the tag which is exactly the same as the way working in browser. However, since weex events are actually triggered directly by native components, the behavior and content of events are different with what exsiting in the browser.

+ Not all types of event are supported, please refer [Common Events](./common-events.html) for more details.
+ There is not difference between catching phase and bubbling phase, which is equivlent to DOM 0 event.
