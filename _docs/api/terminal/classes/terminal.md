---
title: Terminal
category: API-classes
layout: docs
---


# Class: Terminal

The class that represents an xterm.js terminal.

## Hierarchy

**Terminal**

## Implements

* [IEventEmitter]({% link _docs/api/terminal/interfaces/ieventemitter.md %})
* [IDisposable]({% link _docs/api/terminal/interfaces/idisposable.md %})

## Index

### Constructors

* [constructor]({% link _docs/api/terminal/classes/terminal.md %}#constructor)

### Properties

* [cols]({% link _docs/api/terminal/classes/terminal.md %}#cols)
* [element]({% link _docs/api/terminal/classes/terminal.md %}#element)
* [markers]({% link _docs/api/terminal/classes/terminal.md %}#markers)
* [rows]({% link _docs/api/terminal/classes/terminal.md %}#rows)
* [textarea]({% link _docs/api/terminal/classes/terminal.md %}#textarea)
* [strings]({% link _docs/api/terminal/classes/terminal.md %}#strings)

### Methods

* [addCsiHandler]({% link _docs/api/terminal/classes/terminal.md %}#addcsihandler)
* [addDisposableListener]({% link _docs/api/terminal/classes/terminal.md %}#adddisposablelistener)
* [addMarker]({% link _docs/api/terminal/classes/terminal.md %}#addmarker)
* [addOscHandler]({% link _docs/api/terminal/classes/terminal.md %}#addoschandler)
* [attachCustomKeyEventHandler]({% link _docs/api/terminal/classes/terminal.md %}#attachcustomkeyeventhandler)
* [blur]({% link _docs/api/terminal/classes/terminal.md %}#blur)
* [clear]({% link _docs/api/terminal/classes/terminal.md %}#clear)
* [clearSelection]({% link _docs/api/terminal/classes/terminal.md %}#clearselection)
* [deregisterCharacterJoiner]({% link _docs/api/terminal/classes/terminal.md %}#deregistercharacterjoiner)
* [deregisterLinkMatcher]({% link _docs/api/terminal/classes/terminal.md %}#deregisterlinkmatcher)
* [destroy]({% link _docs/api/terminal/classes/terminal.md %}#destroy)
* [dispose]({% link _docs/api/terminal/classes/terminal.md %}#dispose)
* [emit]({% link _docs/api/terminal/classes/terminal.md %}#emit)
* [focus]({% link _docs/api/terminal/classes/terminal.md %}#focus)
* [getOption]({% link _docs/api/terminal/classes/terminal.md %}#getoption)
* [getSelection]({% link _docs/api/terminal/classes/terminal.md %}#getselection)
* [hasSelection]({% link _docs/api/terminal/classes/terminal.md %}#hasselection)
* [off]({% link _docs/api/terminal/classes/terminal.md %}#off)
* [on]({% link _docs/api/terminal/classes/terminal.md %}#on)
* [open]({% link _docs/api/terminal/classes/terminal.md %}#open)
* [refresh]({% link _docs/api/terminal/classes/terminal.md %}#refresh)
* [registerCharacterJoiner]({% link _docs/api/terminal/classes/terminal.md %}#registercharacterjoiner)
* [registerLinkMatcher]({% link _docs/api/terminal/classes/terminal.md %}#registerlinkmatcher)
* [reset]({% link _docs/api/terminal/classes/terminal.md %}#reset)
* [resize]({% link _docs/api/terminal/classes/terminal.md %}#resize)
* [scrollLines]({% link _docs/api/terminal/classes/terminal.md %}#scrolllines)
* [scrollPages]({% link _docs/api/terminal/classes/terminal.md %}#scrollpages)
* [scrollToBottom]({% link _docs/api/terminal/classes/terminal.md %}#scrolltobottom)
* [scrollToLine]({% link _docs/api/terminal/classes/terminal.md %}#scrolltoline)
* [scrollToTop]({% link _docs/api/terminal/classes/terminal.md %}#scrolltotop)
* [selectAll]({% link _docs/api/terminal/classes/terminal.md %}#selectall)
* [selectLines]({% link _docs/api/terminal/classes/terminal.md %}#selectlines)
* [setOption]({% link _docs/api/terminal/classes/terminal.md %}#setoption)
* [write]({% link _docs/api/terminal/classes/terminal.md %}#write)
* [writeln]({% link _docs/api/terminal/classes/terminal.md %}#writeln)
* [applyAddon]({% link _docs/api/terminal/classes/terminal.md %}#applyaddon)

---

## Constructors

<a id="constructor"></a>

###  constructor

⊕ **new Terminal**(options?: *[ITerminalOptions]({% link _docs/api/terminal/interfaces/iterminaloptions.md %})*): [Terminal]({% link _docs/api/terminal/classes/terminal.md %})

*Defined in [xterm.d.ts:347](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L347)*

Creates a new `Terminal` object.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| `Optional` options | [ITerminalOptions]({% link _docs/api/terminal/interfaces/iterminaloptions.md %}) |  An object containing a set of options. |

**Returns:** [Terminal]({% link _docs/api/terminal/classes/terminal.md %})

___

## Properties

<a id="cols"></a>

###  cols

**● cols**: *`number`*

*Defined in [xterm.d.ts:336](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L336)*

The number of columns in the terminal's viewport. Use `ITerminalOptions.cols` to set this in the constructor and `Terminal.resize` for when the terminal exists.

___
<a id="element"></a>

###  element

**● element**: *`HTMLElement`*

*Defined in [xterm.d.ts:317](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L317)*

The element containing the terminal.

___
<a id="markers"></a>

###  markers

**● markers**: *[IMarker]({% link _docs/api/terminal/interfaces/imarker.md %})[]*

*Defined in [xterm.d.ts:342](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L342)*

(EXPERIMENTAL) Get all markers registered against the buffer. If the alt buffer is active this will always return \[\].

___
<a id="rows"></a>

###  rows

**● rows**: *`number`*

*Defined in [xterm.d.ts:329](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L329)*

The number of rows in the terminal's viewport. Use `ITerminalOptions.rows` to set this in the constructor and `Terminal.resize` for when the terminal exists.

___
<a id="textarea"></a>

###  textarea

**● textarea**: *`HTMLTextAreaElement`*

*Defined in [xterm.d.ts:322](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L322)*

The textarea that accepts input for the terminal.

___
<a id="strings"></a>

### `<Static>` strings

**● strings**: *[ILocalizableStrings]({% link _docs/api/terminal/interfaces/ilocalizablestrings.md %})*

*Defined in [xterm.d.ts:347](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L347)*

Natural language strings that can be localized.

___

## Methods

<a id="addcsihandler"></a>

###  addCsiHandler

▸ **addCsiHandler**(flag: *`string`*, callback: *`function`*): [IDisposable]({% link _docs/api/terminal/interfaces/idisposable.md %})

*Defined in [xterm.d.ts:490](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L490)*

(EXPERIMENTAL) Adds a handler for CSI escape sequences.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| flag | `string` |  The flag should be one-character string, which specifies the final character (e.g "m" for SGR) of the CSI sequence. |
| callback | `function` |  The function to handle the escape sequence. The callback is called with the numerical params, as well as the special characters (e.g. "$" for DECSCPP). Return true if the sequence was handled; false if we should try a previous handler (set by addCsiHandler or setCsiHandler). The most recently-added handler is tried first. |

**Returns:** [IDisposable]({% link _docs/api/terminal/interfaces/idisposable.md %})
An IDisposable you can call to remove this handler.

___
<a id="adddisposablelistener"></a>

###  addDisposableListener

▸ **addDisposableListener**(type: *`string`*, handler: *`function`*): [IDisposable]({% link _docs/api/terminal/interfaces/idisposable.md %})

*Defined in [xterm.d.ts:443](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L443)*

Adds an event listener to the Terminal, returning an IDisposable that can be used to conveniently remove the event listener.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| type | `string` |  The type of event. |
| handler | `function` |  The event handler. |

**Returns:** [IDisposable]({% link _docs/api/terminal/interfaces/idisposable.md %})

___
<a id="addmarker"></a>

###  addMarker

▸ **addMarker**(cursorYOffset: *`number`*): [IMarker]({% link _docs/api/terminal/interfaces/imarker.md %})

*Defined in [xterm.d.ts:563](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L563)*

(EXPERIMENTAL) Adds a marker to the normal buffer and returns it. If the alt buffer is active, undefined is returned.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| cursorYOffset | `number` |  The y position offset of the marker from the cursor. |

**Returns:** [IMarker]({% link _docs/api/terminal/interfaces/imarker.md %})

___
<a id="addoschandler"></a>

###  addOscHandler

▸ **addOscHandler**(ident: *`number`*, callback: *`function`*): [IDisposable]({% link _docs/api/terminal/interfaces/idisposable.md %})

*Defined in [xterm.d.ts:501](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L501)*

(EXPERIMENTAL) Adds a handler for OSC escape sequences.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| ident | `number` |  The number (first parameter) of the sequence. |
| callback | `function` |  The function to handle the escape sequence. The callback is called with OSC data string. Return true if the sequence was handled; false if we should try a previous handler (set by addOscHandler or setOscHandler). The most recently-added handler is tried first. |

**Returns:** [IDisposable]({% link _docs/api/terminal/interfaces/idisposable.md %})
An IDisposable you can call to remove this handler.

___
<a id="attachcustomkeyeventhandler"></a>

###  attachCustomKeyEventHandler

▸ **attachCustomKeyEventHandler**(customKeyEventHandler: *`function`*): `void`

*Defined in [xterm.d.ts:477](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L477)*

Attaches a custom key event handler which is run before keys are processed, giving consumers of xterm.js ultimate control as to what keys should be processed by the terminal and what keys should not.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| customKeyEventHandler | `function` |  The custom KeyboardEvent handler to attach. This is a function that takes a KeyboardEvent, allowing consumers to stop propagation and/or prevent the default action. The function returns whether the event should be processed by xterm.js. |

**Returns:** `void`

___
<a id="blur"></a>

###  blur

▸ **blur**(): `void`

*Defined in [xterm.d.ts:359](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L359)*

Unfocus the terminal.

**Returns:** `void`

___
<a id="clear"></a>

###  clear

▸ **clear**(): `void`

*Defined in [xterm.d.ts:637](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L637)*

Clear the entire buffer, making the prompt line the new first line.

**Returns:** `void`

___
<a id="clearselection"></a>

###  clearSelection

▸ **clearSelection**(): `void`

*Defined in [xterm.d.ts:579](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L579)*

Clears the current terminal selection.

**Returns:** `void`

___
<a id="deregistercharacterjoiner"></a>

###  deregisterCharacterJoiner

▸ **deregisterCharacterJoiner**(joinerId: *`number`*): `void`

*Defined in [xterm.d.ts:556](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L556)*

(EXPERIMENTAL) Deregisters the character joiner if one was registered. NOTE: character joiners are only used by the canvas renderer.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| joinerId | `number` |  The character joiner's ID (returned after register) |

**Returns:** `void`

___
<a id="deregisterlinkmatcher"></a>

###  deregisterLinkMatcher

▸ **deregisterLinkMatcher**(matcherId: *`number`*): `void`

*Defined in [xterm.d.ts:518](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L518)*

(EXPERIMENTAL) Deregisters a link matcher if it has been registered.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| matcherId | `number` |  The link matcher's ID (returned after register) |

**Returns:** `void`

___
<a id="destroy"></a>

###  destroy

▸ **destroy**(): `void`

*Defined in [xterm.d.ts:604](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L604)*

Destroys the terminal and detaches it from the DOM.

*__deprecated__*:
 Use dispose() instead.

**Returns:** `void`

___
<a id="dispose"></a>

###  dispose

▸ **dispose**(): `void`

*Implementation of [IDisposable]({% link _docs/api/terminal/interfaces/idisposable.md %}).[dispose]({% link _docs/api/terminal/interfaces/idisposable.md %}#dispose)*

*Defined in [xterm.d.ts:597](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L597)*

**Returns:** `void`

___
<a id="emit"></a>

###  emit

▸ **emit**(type: *`string`*, data?: *`any`*): `void`

*Implementation of [IEventEmitter]({% link _docs/api/terminal/interfaces/ieventemitter.md %}).[emit]({% link _docs/api/terminal/interfaces/ieventemitter.md %}#emit)*

*Defined in [xterm.d.ts:435](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L435)*

Emits an event on the terminal.

*__deprecated__*:
 This is being removed from the API with no replacement, see issue #1505.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| type | `string` |  The type of event |
| `Optional` data | `any` |  data associated with the event. |

**Returns:** `void`

___
<a id="focus"></a>

###  focus

▸ **focus**(): `void`

*Defined in [xterm.d.ts:364](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L364)*

Focus the terminal.

**Returns:** `void`

___
<a id="getoption"></a>

###  getOption

▸ **getOption**(key: *"bellSound" \| "bellStyle" \| "cursorStyle" \| "fontFamily" \| "fontWeight" \| "fontWeightBold" \| "rendererType" \| "termName"*): `string`

▸ **getOption**(key: *"allowTransparency" \| "cancelEvents" \| "convertEol" \| "cursorBlink" \| "debug" \| "disableStdin" \| "enableBold" \| "macOptionIsMeta" \| "rightClickSelectsWord" \| "popOnBell" \| "screenKeys" \| "useFlowControl" \| "visualBell"*): `boolean`

▸ **getOption**(key: *"colors"*): `string`[]

▸ **getOption**(key: *"cols" \| "fontSize" \| "letterSpacing" \| "lineHeight" \| "rows" \| "tabStopWidth" \| "scrollback"*): `number`

▸ **getOption**(key: *"handler"*): `function`

▸ **getOption**(key: *`string`*): `any`

*Defined in [xterm.d.ts:649](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L649)*

Retrieves an option's value from the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | "bellSound" \| "bellStyle" \| "cursorStyle" \| "fontFamily" \| "fontWeight" \| "fontWeightBold" \| "rendererType" \| "termName" |  The option key. |

**Returns:** `string`

*Defined in [xterm.d.ts:654](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L654)*

Retrieves an option's value from the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | "allowTransparency" \| "cancelEvents" \| "convertEol" \| "cursorBlink" \| "debug" \| "disableStdin" \| "enableBold" \| "macOptionIsMeta" \| "rightClickSelectsWord" \| "popOnBell" \| "screenKeys" \| "useFlowControl" \| "visualBell" |  The option key. |

**Returns:** `boolean`

*Defined in [xterm.d.ts:659](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L659)*

Retrieves an option's value from the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | "colors" |  The option key. |

**Returns:** `string`[]

*Defined in [xterm.d.ts:664](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L664)*

Retrieves an option's value from the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | "cols" \| "fontSize" \| "letterSpacing" \| "lineHeight" \| "rows" \| "tabStopWidth" \| "scrollback" |  The option key. |

**Returns:** `number`

*Defined in [xterm.d.ts:669](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L669)*

Retrieves an option's value from the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | "handler" |  The option key. |

**Returns:** `function`

*Defined in [xterm.d.ts:674](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L674)*

Retrieves an option's value from the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | `string` |  The option key. |

**Returns:** `any`

___
<a id="getselection"></a>

###  getSelection

▸ **getSelection**(): `string`

*Defined in [xterm.d.ts:574](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L574)*

Gets the terminal's current selection, this is useful for implementing copy behavior outside of xterm.js.

**Returns:** `string`

___
<a id="hasselection"></a>

###  hasSelection

▸ **hasSelection**(): `boolean`

*Defined in [xterm.d.ts:568](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L568)*

Gets whether the terminal has an active selection.

**Returns:** `boolean`

___
<a id="off"></a>

###  off

▸ **off**(type: *"blur" \| "focus" \| "linefeed" \| "selection" \| "data" \| "key" \| "keypress" \| "keydown" \| "refresh" \| "resize" \| "scroll" \| "title" \| `string`*, listener: *`function`*): `void`

*Defined in [xterm.d.ts:426](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L426)*

Deregisters an event listener.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| type | "blur" \| "focus" \| "linefeed" \| "selection" \| "data" \| "key" \| "keypress" \| "keydown" \| "refresh" \| "resize" \| "scroll" \| "title" \| `string` |  The type of the event. |
| listener | `function` |  The listener. |

**Returns:** `void`

___
<a id="on"></a>

###  on

▸ **on**(type: *"blur" \| "focus" \| "linefeed" \| "selection"*, listener: *`function`*): `void`

▸ **on**(type: *"data"*, listener: *`function`*): `void`

▸ **on**(type: *"key"*, listener: *`function`*): `void`

▸ **on**(type: *"keypress" \| "keydown"*, listener: *`function`*): `void`

▸ **on**(type: *"refresh"*, listener: *`function`*): `void`

▸ **on**(type: *"resize"*, listener: *`function`*): `void`

▸ **on**(type: *"scroll"*, listener: *`function`*): `void`

▸ **on**(type: *"title"*, listener: *`function`*): `void`

▸ **on**(type: *`string`*, listener: *`function`*): `void`

*Defined in [xterm.d.ts:371](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L371)*

Registers an event listener.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| type | "blur" \| "focus" \| "linefeed" \| "selection" |  The type of the event. |
| listener | `function` |  The listener. |

**Returns:** `void`

*Defined in [xterm.d.ts:377](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L377)*

Registers an event listener.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| type | "data" |  The type of the event. |
| listener | `function` |  The listener. |

**Returns:** `void`

*Defined in [xterm.d.ts:383](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L383)*

Registers an event listener.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| type | "key" |  The type of the event. |
| listener | `function` |  The listener. |

**Returns:** `void`

*Defined in [xterm.d.ts:389](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L389)*

Registers an event listener.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| type | "keypress" \| "keydown" |  The type of the event. |
| listener | `function` |  The listener. |

**Returns:** `void`

*Defined in [xterm.d.ts:395](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L395)*

Registers an event listener.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| type | "refresh" |  The type of the event. |
| listener | `function` |  The listener. |

**Returns:** `void`

*Defined in [xterm.d.ts:401](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L401)*

Registers an event listener.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| type | "resize" |  The type of the event. |
| listener | `function` |  The listener. |

**Returns:** `void`

*Defined in [xterm.d.ts:407](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L407)*

Registers an event listener.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| type | "scroll" |  The type of the event. |
| listener | `function` |  The listener. |

**Returns:** `void`

*Defined in [xterm.d.ts:413](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L413)*

Registers an event listener.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| type | "title" |  The type of the event. |
| listener | `function` |  The listener. |

**Returns:** `void`

*Defined in [xterm.d.ts:419](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L419)*

Registers an event listener.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| type | `string` |  The type of the event. |
| listener | `function` |  The listener. |

**Returns:** `void`

___
<a id="open"></a>

###  open

▸ **open**(parent: *`HTMLElement`*): `void`

*Defined in [xterm.d.ts:466](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L466)*

Opens the terminal within an element.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| parent | `HTMLElement` |  The element to create the terminal within. This element must be visible (have dimensions) when \`open\` is called as several DOM- based measurements need to be performed when this function is called. |

**Returns:** `void`

___
<a id="refresh"></a>

###  refresh

▸ **refresh**(start: *`number`*, end: *`number`*): `void`

*Defined in [xterm.d.ts:749](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L749)*

Tells the renderer to refresh terminal content between two rows (inclusive) at the next opportunity.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| start | `number` |  The row to start from (between 0 and this.rows - 1). |
| end | `number` |  The row to end at (between start and this.rows - 1). |

**Returns:** `void`

___
<a id="registercharacterjoiner"></a>

###  registerCharacterJoiner

▸ **registerCharacterJoiner**(handler: *`function`*): `number`

*Defined in [xterm.d.ts:549](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L549)*

(EXPERIMENTAL) Registers a character joiner, allowing custom sequences of characters to be rendered as a single unit. This is useful in particular for rendering ligatures and graphemes, among other things.

Each registered character joiner is called with a string of text representing a portion of a line in the terminal that can be rendered as a single unit. The joiner must return a sorted array, where each entry is itself an array of length two, containing the start (inclusive) and end (exclusive) index of a substring of the input that should be rendered as a single unit. When multiple joiners are provided, the results of each are collected. If there are any overlapping substrings between them, they are combined into one larger unit that is drawn together.

All character joiners that are registered get called every time a line is rendered in the terminal, so it is essential for the handler function to run as quickly as possible to avoid slowdowns when rendering. Similarly, joiners should strive to return the smallest possible substrings to render together, since they aren't drawn as optimally as individual characters.

NOTE: character joiners are only used by the canvas renderer.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| handler | `function` |  The function that determines character joins. It is called with a string of text that is eligible for joining and returns an array where each entry is an array containing the start (inclusive) and end (exclusive) indexes of ranges that should be rendered as a single unit. |

**Returns:** `number`
The ID of the new joiner, this can be used to deregister

___
<a id="registerlinkmatcher"></a>

###  registerLinkMatcher

▸ **registerLinkMatcher**(regex: *`RegExp`*, handler: *`function`*, options?: *[ILinkMatcherOptions]({% link _docs/api/terminal/interfaces/ilinkmatcheroptions.md %})*): `number`

*Defined in [xterm.d.ts:512](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L512)*

(EXPERIMENTAL) Registers a link matcher, allowing custom link patterns to be matched and handled.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| regex | `RegExp` |  The regular expression to search for, specifically this searches the textContent of the rows. You will want to use \\s to match a space ' ' character for example. |
| handler | `function` |  The callback when the link is called. |
| `Optional` options | [ILinkMatcherOptions]({% link _docs/api/terminal/interfaces/ilinkmatcheroptions.md %}) |  Options for the link matcher. |

**Returns:** `number`
The ID of the new matcher, this can be used to deregister.

___
<a id="reset"></a>

###  reset

▸ **reset**(): `void`

*Defined in [xterm.d.ts:754](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L754)*

Perform a full reset (RIS, aka '\\x1bc').

**Returns:** `void`

___
<a id="resize"></a>

###  resize

▸ **resize**(columns: *`number`*, rows: *`number`*): `void`

*Defined in [xterm.d.ts:452](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L452)*

Resizes the terminal. It's best practice to debounce calls to resize, this will help ensure that the pty can respond to the resize event before another one occurs.

**Parameters:**

| Name | Type |
| ------ | ------ |
| columns | `number` |
| rows | `number` |

**Returns:** `void`

___
<a id="scrolllines"></a>

###  scrollLines

▸ **scrollLines**(amount: *`number`*): `void`

*Defined in [xterm.d.ts:610](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L610)*

Scroll the display of the terminal

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| amount | `number` |  The number of lines to scroll down (negative scroll up). |

**Returns:** `void`

___
<a id="scrollpages"></a>

###  scrollPages

▸ **scrollPages**(pageCount: *`number`*): `void`

*Defined in [xterm.d.ts:616](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L616)*

Scroll the display of the terminal by a number of pages.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| pageCount | `number` |  The number of pages to scroll (negative scrolls up). |

**Returns:** `void`

___
<a id="scrolltobottom"></a>

###  scrollToBottom

▸ **scrollToBottom**(): `void`

*Defined in [xterm.d.ts:626](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L626)*

Scrolls the display of the terminal to the bottom.

**Returns:** `void`

___
<a id="scrolltoline"></a>

###  scrollToLine

▸ **scrollToLine**(line: *`number`*): `void`

*Defined in [xterm.d.ts:632](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L632)*

Scrolls to a line within the buffer.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| line | `number` |  The 0-based line index to scroll to. |

**Returns:** `void`

___
<a id="scrolltotop"></a>

###  scrollToTop

▸ **scrollToTop**(): `void`

*Defined in [xterm.d.ts:621](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L621)*

Scrolls the display of the terminal to the top.

**Returns:** `void`

___
<a id="selectall"></a>

###  selectAll

▸ **selectAll**(): `void`

*Defined in [xterm.d.ts:584](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L584)*

Selects all text within the terminal.

**Returns:** `void`

___
<a id="selectlines"></a>

###  selectLines

▸ **selectLines**(start: *`number`*, end: *`number`*): `void`

*Defined in [xterm.d.ts:591](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L591)*

Selects text in the buffer between 2 lines.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| start | `number` |  The 0-based line index to select from (inclusive). |
| end | `number` |  The 0-based line index to select to (inclusive). |

**Returns:** `void`

___
<a id="setoption"></a>

###  setOption

▸ **setOption**(key: *"fontFamily" \| "termName" \| "bellSound"*, value: *`string`*): `void`

▸ **setOption**(key: *"fontWeight" \| "fontWeightBold"*, value: *`null` \| "normal" \| "bold" \| "100" \| "200" \| "300" \| "400" \| "500" \| "600" \| "700" \| "800" \| "900"*): `void`

▸ **setOption**(key: *"bellStyle"*, value: *`null` \| "none" \| "visual" \| "sound" \| "both"*): `void`

▸ **setOption**(key: *"cursorStyle"*, value: *`null` \| "block" \| "underline" \| "bar"*): `void`

▸ **setOption**(key: *"allowTransparency" \| "cancelEvents" \| "convertEol" \| "cursorBlink" \| "debug" \| "disableStdin" \| "enableBold" \| "macOptionIsMeta" \| "popOnBell" \| "rightClickSelectsWord" \| "screenKeys" \| "useFlowControl" \| "visualBell"*, value: *`boolean`*): `void`

▸ **setOption**(key: *"colors"*, value: *`string`[]*): `void`

▸ **setOption**(key: *"fontSize" \| "letterSpacing" \| "lineHeight" \| "tabStopWidth" \| "scrollback"*, value: *`number`*): `void`

▸ **setOption**(key: *"handler"*, value: *`function`*): `void`

▸ **setOption**(key: *"theme"*, value: *[ITheme]({% link _docs/api/terminal/interfaces/itheme.md %})*): `void`

▸ **setOption**(key: *"cols" \| "rows"*, value: *`number`*): `void`

▸ **setOption**(key: *`string`*, value: *`any`*): `void`

*Defined in [xterm.d.ts:681](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L681)*

Sets an option on the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | "fontFamily" \| "termName" \| "bellSound" |  The option key. |
| value | `string` |  The option value. |

**Returns:** `void`

*Defined in [xterm.d.ts:687](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L687)*

Sets an option on the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | "fontWeight" \| "fontWeightBold" |  The option key. |
| value | `null` \| "normal" \| "bold" \| "100" \| "200" \| "300" \| "400" \| "500" \| "600" \| "700" \| "800" \| "900" |  The option value. |

**Returns:** `void`

*Defined in [xterm.d.ts:693](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L693)*

Sets an option on the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | "bellStyle" |  The option key. |
| value | `null` \| "none" \| "visual" \| "sound" \| "both" |  The option value. |

**Returns:** `void`

*Defined in [xterm.d.ts:699](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L699)*

Sets an option on the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | "cursorStyle" |  The option key. |
| value | `null` \| "block" \| "underline" \| "bar" |  The option value. |

**Returns:** `void`

*Defined in [xterm.d.ts:705](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L705)*

Sets an option on the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | "allowTransparency" \| "cancelEvents" \| "convertEol" \| "cursorBlink" \| "debug" \| "disableStdin" \| "enableBold" \| "macOptionIsMeta" \| "popOnBell" \| "rightClickSelectsWord" \| "screenKeys" \| "useFlowControl" \| "visualBell" |  The option key. |
| value | `boolean` |  The option value. |

**Returns:** `void`

*Defined in [xterm.d.ts:711](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L711)*

Sets an option on the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | "colors" |  The option key. |
| value | `string`[] |  The option value. |

**Returns:** `void`

*Defined in [xterm.d.ts:717](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L717)*

Sets an option on the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | "fontSize" \| "letterSpacing" \| "lineHeight" \| "tabStopWidth" \| "scrollback" |  The option key. |
| value | `number` |  The option value. |

**Returns:** `void`

*Defined in [xterm.d.ts:723](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L723)*

Sets an option on the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | "handler" |  The option key. |
| value | `function` |  The option value. |

**Returns:** `void`

*Defined in [xterm.d.ts:729](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L729)*

Sets an option on the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | "theme" |  The option key. |
| value | [ITheme]({% link _docs/api/terminal/interfaces/itheme.md %}) |  The option value. |

**Returns:** `void`

*Defined in [xterm.d.ts:735](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L735)*

Sets an option on the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | "cols" \| "rows" |  The option key. |
| value | `number` |  The option value. |

**Returns:** `void`

*Defined in [xterm.d.ts:741](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L741)*

Sets an option on the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| key | `string` |  The option key. |
| value | `any` |  The option value. |

**Returns:** `void`

___
<a id="write"></a>

###  write

▸ **write**(data: *`string`*): `void`

*Defined in [xterm.d.ts:643](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L643)*

Writes text to the terminal.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| data | `string` |  The text to write to the terminal. |

**Returns:** `void`

___
<a id="writeln"></a>

###  writeln

▸ **writeln**(data: *`string`*): `void`

*Defined in [xterm.d.ts:458](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L458)*

Writes text to the terminal, followed by a break line character (\\n).

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| data | `string` |  The text to write to the terminal. |

**Returns:** `void`

___
<a id="applyaddon"></a>

### `<Static>` applyAddon

▸ **applyAddon**(addon: *`any`*): `void`

*Defined in [xterm.d.ts:761](https://github.com/xtermjs/xterm.js/blob/3.12.0/typings/xterm.d.ts#L761)*

Applies an addon to the Terminal prototype, making it available to all newly created Terminals.

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| addon | `any` |  The addon to apply. |

**Returns:** `void`

___

