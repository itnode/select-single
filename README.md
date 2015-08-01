# select-single

An element to provide a select for huge value lists. It is requesting an Backend URL to fetch matching list items and shows them.
Keyboard and Mouse can be used to select an Entry. The defined Entry Value will be placed in a hidden input in the ShadowDOM to 
provide the Value per HTTP Requst.

## Synopsis

    <select-single backend="http://private-c3fe6-selectsingle.apiary-mock.com/items" name="member_id" selected='{"title": "Lord Meowser", "id": "9999" }'>
    </select-single>

The *backend* Attribute stores the provided Backend JSON.
The *selected* Attribute stores the JSON of the selected Entry. You can provide a Default with it.

## Screenshots

The Search Box:

![The Search](https://raw.githubusercontent.com/itnode/select-single/master/screenshots/001.png)

The Value List:

![Value List](https://raw.githubusercontent.com/itnode/select-single/master/screenshots/002.png)

The Selected Entry

![Selected Entry](https://raw.githubusercontent.com/itnode/select-single/master/screenshots/003.png)

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install


## Playing With Your Element

If you wish to work on your element in isolation, we recommend that you use
[Polyserve](https://github.com/PolymerLabs/polyserve) to keep your element's
bower dependencies in line. You can install it via:

    npm install -g polyserve

And you can run it via:

    polyserve

Once running, you can preview your element at
`http://localhost:8080/components/select-single/`, where `select-single` is the name of the directory containing it.


## Testing Your Element

Simply navigate to the `/test` directory of your element to run its tests. If
you are using Polyserve: `http://localhost:8080/components/select-single/test/`

### web-component-tester

The tests are compatible with [web-component-tester](https://github.com/Polymer/web-component-tester).
Install it via:

    npm install -g web-component-tester

Then, you can run your tests on _all_ of your local browsers via:

    wct

#### WCT Tips

`wct -l chrome` will only run tests in chrome.

`wct -p` will keep the browsers alive after test runs (refresh to re-run).

`wct test/some-file.html` will test only the files you specify.
