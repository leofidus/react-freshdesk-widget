# react-freshdesk-widget [![Build Status](https://scrutinizer-ci.com/g/Personare/react-freshdesk-widget/badges/build.png?b=master&s=6b40b4cc955a743a38efda66164a0ee2659d945f)](https://scrutinizer-ci.com/g/Personare/react-freshdesk-widget/build-status/master)

> A component of React for use the Freshdesk Widget 

<br />

<p align="center">
  <img width="50%" src="./docs/freshdesk.png?raw=true" alt="Freshdesk Logotype" />
</p>

<br />

## Installation 

```bash
npm install @personare/react-freshdesk-widget --save
```

## Basic Usage

```js
import FreshdeskWidget from '@personare/react-freshdesk-widget';

<FreshdeskWidget url="https://support.freshdesk.com" />
```

## Props

* [`url`](#urlProperty)
* [`type`](#typeProperty)
* [`formTitle`](#formTitleProperty)
* [`formHeight`](#formHeightProperty)
* [`submitThanks`](#submitThanksProperty)

<a name="urlProperty"></a>

#### `url` (required)

An URL of the service of your Freshdesk

For example:

```js

...
render() {
    const urlService = "https://support.freshdesk.com";
    
    return (
        <FreshdeskWidget url="{urlService}" />
    );
}
...

```

<a name="typeProperty"></a>

#### `type` - one of ['pop-up', 'incorporated']

The type of widget you want to insert the page.

Currently you can perform through two ways:

1. Through a pop-up where the user must click to display the widget.
2. Incorporating direct in your HTML.

*default: incorporated*

For example:

```js
...

render() {
    return (
        <FreshdeskWidget 
            url="https://support.freshdesk.com"
            type="pop-up"
        />
    );
}

...
```

<a name="formTitleProperty"></a>

#### `formTitle`

What will be the title of the form.

*default: Help and support*

For example:

```js
...

render() {
    return (
        <FreshdeskWidget 
            url="https://support.freshdesk.com"
            formTitle="This is a custom title"
        />
    );
}

...
```

<a name="formHeightProperty"></a>

#### `formHeight`

The height of the form.

*default: 500px*

For example:

```js
...

render() {
    return (
        <FreshdeskWidget 
            url="https://support.freshdesk.com"
            formHeight="700px"
        />
    );
}

...
```

<a name="submitThanksProperty"></a>

#### `submitThanks`

The message that appears after the user send feedback.

*default: Thank you, one of our representatives will respond to you soon! =)*

For example:

```js
...

render() {
    return (
        <FreshdeskWidget 
            url="https://support.freshdesk.com"
            submitThanks="Thank you!!!"
        />
    );
}

...
```

## Development

To start developing in the project run:

```bash
npm run serve
```

Then ready at `http://localhost:9001`.

## Tests

Just run:

```bash
npm run tests
```

<br />

*This scaffolding will be generated by* [@Personare/react-component-generator](https://github.com/Personare/react-component-generator)
