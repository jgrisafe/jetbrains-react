# jetbrains-react

React snippets([live templates](https://www.jetbrains.com/help/idea/2016.1/live-templates.html)) for JetBrains series editors (e.g. WebStorm, PHPStorm, IntelliJ IDEA, etc.), stolen from [sublime-react](https://github.com/reactjs/sublime-react) and [phpstorm-reactjs](https://github.com/geochatz/phpstorm-reactjs).

## Installation

### Import Automatically

1. Download [**`settings.jar`**](https://github.com/minwe/jetbrains-react/raw/master/settings.jar);
2. Click `File` -> `Importing Settings...` on your IDE menu, select `settings.jar`, then click `OK`.

### Install Manually

1. Download([save as...](https://raw.githubusercontent.com/minwe/jetbrains-react/master/jetbrains/templates/ReactJS.xml)) and copy the `jetbrains/templates/ReactJS.xml` file to your templates folder:

  - Windows: `<your home directory>\.<product name><version number>\config\templates`
  - Linux: `~\.<product name><version number>\config\templates`
  - OS X: `~/Library/Preferences/<product name><version number>/templates`

  e.g. `~/Library/Preferences/WebStorm10/templates` on OS X for WebStorm 10

2. Restart your IDE.

3. To see all templates, go to `Preferences` -> `Live Templates` and expand the `ReactJS` Template Group.


## Usage

It's hard to remember shortcuts when there are a large number of options. A more efficient way is to take advantage of editor's Insert Live Template shortcut. Press `Cmd + J` and type as many letters as you want to filter the results.

For example, to create a new React class, type `rcc` and press `Tab` or press `Cmd + J` and write `rcc` or `React`.

**The WebStorm official blog post**:

- [Working with ReactJS in WebStorm: Coding Assistance](http://blog.jetbrains.com/webstorm/2015/10/working-with-reactjs-in-webstorm-coding-assistance/)

**Documentation of available snippets:**

<!--DOC_START-->
### `rcc`

```js
import React, { Component, PropTypes } from 'react';

class $COMPONENT$ extends Component {
  render() {
    return (
      <div>$END$</div>
    )
  }
}

$COMPONENT$.propTypes = {}
$COMPONENT$.defaultProps = {}

export default $COMPONENT$

```

### `rpfc`

```js
import React, { PropTypes } from 'react'

const $COMPONENT$ = ($PARAMETER$) => {
  return (
    <div>$END$</div>
  )
}

$COMPONENT$.propTypes = {}
$COMPONENT$.defaultProps = {}

export default $COMPONENT$

```

### `rdom`

```js
import ReactDOM from 'react-dom';
$END$

```

### `cdm`

```js
componentDidMount() {
  $END$
}

```

### `cdu`

```js
componentDidUpdate(prevProps, prevState) {
  $END$
}

```

### `cwm`

```js
componentWillMount() {
  $END$
}

```

### `cwr`

```js
componentWillReceiveProps(nextProps, nextContext) {
  $END$
}

```

### `cwu`

```js
componentWillUpdate(nextProps, nextState) {
  $END$
}

```

### `cwum`

```js
componentWillUnmount() {
  $END$
}

```

### `props`

```js
this.props
```

### `dsih`

```js
dangerouslySetInnerHTML={{__html: '$END$'}}
```

### `pt`

```js
$START$: PropTypes.$END$,
```

### `ren`

```js
render() {
  return (
    <div>$END$</div>
  )
}

```

### `scu`

```js
shouldComponentUpdate(nextProps, nextState) {
  $END$
}

```

### `sst`

```js
this.setState({ $START$: $END$ })

```

### `cstt`

```js
constructor(props) {
  super(props)
  $END$
}

```

### `tsn`

```js
transitionName="$END$"
```

### `tsa`

```js
transitionAppear={$END$}
```

### `tse`

```js
transitionEnter={$END$}
```

### `tsl`

```js
transitionLeave={$END$}
```

### `tset`

```js
transitionEnterTimeout={$END$}
```

### `tslt`

```js
transitionLeaveTimeout={$END$}
```

### `tsat`

```js
transitionAppearTimeout={$END$}
```

### `oncp`

```js
onCopy={$END$}
```

### `onct`

```js
onCut={$END$}
```

### `onpt`

```js
onPaste={$END$}
```

### `oncpse`

```js
onCompositionEnd={$END$}
```

### `oncpss`

```js
onCompositionStart={$END$}
```

### `oncpsu`

```js
onCompositionUpdate={$END$}
```

### `onkd`

```js
onKeyDown={$END$}
```

### `onps`

```js
onKeyPress={$END$}
```

### `onku`

```js
onKeyUp={$END$}
```

### `onfs`

```js
onFocus={$END$}
```

### `onbl`

```js
onBlur={$END$}
```

### `oncg`

```js
onChange={$END$}
```

### `onip`

```js
onInput={$END$}
```

### `onsb`

```js
onSubmit={$END$}
```

### `onc`

```js
onClick={$END$}
```

### `oncm`

```js
onContextMenu={$END$}
```

### `ondc`

```js
onDoubleClick={$END$}
```

### `ondg`

```js
onDrag={$END$}
```

### `ondge`

```js
onDragEnd={$END$}
```

### `ondgetr`

```js
onDragEnter={$END$}
```

### `ondget`

```js
onDragExit={$END$}
```

### `ondgl`

```js
onDragLeave={$END$}
```

### `ondgo`

```js
onDragOver={$END$}
```

### `ondgst`

```js
onDragStart={$END$}
```

### `ondp`

```js
onDrop={$END$}
```

### `onmd`

```js
onMouseDown={$END$}
```

### `onme`

```js
onMouseEnter={$END$}
```

### `onml`

```js
onMouseLeave={$END$}
```

### `onmm`

```js
onMouseMove={$END$}
```

### `onmot`

```js
onMouseOut={$END$}
```

### `onmov`

```js
onMouseOver={$END$}
```

### `onmu`

```js
onMouseUp={$END$}
```

### `onsl`

```js
onSelect={$END$}
```

### `ontc`

```js
onTouchCancel={$END$}
```

### `onte`

```js
onTouchEnd={$END$}
```

### `ontm`

```js
onTouchMove={$END$}
```

### `onts`

```js
onTouchStart={$END$}
```

### `onsl`

```js
onScroll={$END$}
```

### `onwl`

```js
onWheel={$END$}
```

### `onabt`

```js
onAbort={$END$}
```

### `oncpl`

```js
onCanPlay={$END$}
```

### `oncpt`

```js
onCanPlayThrough={$END$}
```

### `ondc`

```js
onDurationChange={$END$}
```

### `onempt`

```js
onEmptied={$END$}
```

### `onekpt`

```js
onEncrypted={$END$}
```

### `onend`

```js
onEnded={$END$}
```

### `onldd`

```js
onLoadedData={$END$}
```

### `onldmd`

```js
onLoadedMetadata={$END$}
```

### `onls`

```js
onLoadStart={$END$}
```

### `onpaus`

```js
onPause={$END$}
```

### `opl`

```js
onPlay={$END$}
```

### `onplg`

```js
onPlaying={$END$}
```

### `onpgs`

```js
onProgress={$END$}
```

### `onrc`

```js
onRateChange={$END$}
```

### `onsked`

```js
onSeeked={$END$}
```

### `onskin`

```js
onSeeking={$END$}
```

### `onstd`

```js
onStalled={$END$}
```

### `onsupd`

```js
onSuspend={$END$}
```

### `ontu`

```js
onTimeUpdate={$END$}
```

### `onvc`

```js
onVolumeChange={$END$}
```

### `onwt`

```js
onWaiting={$END$}
```

### `onld`

```js
onLoad={$END$}
```

### `onerr`

```js
onError={$END$}
```

### `onas`

```js
onAnimationStart={$END$}
```

### `onae`

```js
onAnimationEnd={$END$}
```

### `onai`

```js
onAnimationIteration={$END$}
```

### `ontse`

```js
onTransitionEnd={$END$}
```


<!--DOC_END-->
