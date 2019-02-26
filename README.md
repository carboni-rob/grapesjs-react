GrapesJS React Integration
==========================
_The first integration of GrapesJS for React._

1. Installation
    - YARN
    ```bash
    yarn add grapesjs-react
    ```
    - NPM
    ```bash
    $ npm install grapesjs-react
    ```
    
2. Usage

    - Class Component:
    ```javascript
    import React, {Component} from 'react';
    import GEditor from 'grapesjs-react';

    class GEditorExample extends Component {
     render() {
       return (
         <GEditor/>
         );
       }
    }
 
    export default GEditorExample;
    ```
    - Functional Component:
    ```javascript
    import React from 'react';
    import GJSEditor from 'grapesjs-react';

    export default function GrapesEditor() {
      return <GJSEditor/>;
    }
    ```

3. Options
The `<GEditor>` component accepts the following props:
    - `newsletter` (boolean - DEFAULT: true): uses the `grapesjs-preset-newsletter` plugin
    - `webpage` (boolean - DEFAULT: false): uses the `grapesjs-preset-webpage` plugin
    - `form` (boolean - DEFAULT: true): whether or not to include the form components in the Block Manager
    - `customCode` (boolean - DEFAULT: true): whether or not to include the Custom Code component in the Block Manager
    - `storageManager` (object): the Storage Manager configuration object
    - `blockManager` (object): the Block Manager configuration object

* This package does not include CSS, so you have to import css from `grapesjs` package manually.

    ```javascript
    import 'grapesjs/dist/css/grapes.min.css';
    ```
* If the peer package is not installed, run the command below:

    ```bash
    yarn add grapesjs
    ```
