---
layout: post
title: React Cheatsheet
---

Anyone who uses React knows one thing, its documentation is pretty frustrating to parse at a high level. To help save my sanity, while working on a small React-based side project, and to save yours, here's a hopefully handy cheatsheet of the core API.

Current as of version **0.11.2**:

* [React](http://facebook.github.io/react/docs/top-level-api.html)
    * createClass(_Object_) -> _function_
    * renderComponent(_ReactComponent_, _DOMElement_, _[function]_) -> _ReactComponent_
    * unmountComponentAtNode(_DOMElement_) -> _Boolean_
    * renderComponentToString(_ReactComponent_) -> _String_
    * renderComponentToStaticMarkup(_ReactComponent_) -> _String_
    * isValidClass(_function (createClass return)_) -> _Boolean_
    * isValidComponent(_Object_)
    * DOM
    * PropTypes
        * array
        * bool
        * func
        * number
        * object
        * string
        * renderable
        * component
        * any
        * _type_.isRequired
        * instanceOf(_class_)
        * oneOf(_[]_)
        * arrayOf(_type_)
        * objectOf(_type_)
        * shape(_object_)
    * initializeTouchEvents(_Boolean_)
    * Children

* [ReactComponent](http://facebook.github.io/react/docs/component-api.html)
    * setState(_Object_, _[function]_)
    * replaceState(_Object_, _[function]_)
    * forceUpdate(_[function]_)
    * getDOMNode() -> _DOMElement_
    * isMounted() -> _Boolean_
    * transferPropsTo(_ReactComponent_) -> _ReactComponent_
    * setProps(_Object_, _[function]_)
    * replaceProps(_Object_, _[function]_)

* [Component Specification](http://facebook.github.io/react/docs/component-specs.html#component-specifications)
    * render() -> _ReactComponent_
    * getInitialState() -> _Object_
    * getDefaultProps() -> _Object_
    * propTypes ~> _{}_
    * mixins ~> _[]_
    * statics ~> _{}_
    * displayName ~> _""_

* [Component Lifecycle Methods](http://facebook.github.io/react/docs/component-specs.html#lifecycle-methods)
    * componentWillMount()
    * componentDidMount()
    * componentWillReceiveProps(_Object_)
    * shouldComponentUpdate(_Object_, _Object_)
    * componentWillUpdate(_Object_, _Object_)
    * componentDidUpdate(_Object_, _Object_)
    * componentWillUnmount()
