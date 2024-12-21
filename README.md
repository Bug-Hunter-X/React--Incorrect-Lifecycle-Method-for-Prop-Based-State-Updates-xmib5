# React Lifecycle Method Bug

This repository demonstrates a common bug in React applications involving the incorrect use of lifecycle methods for updating state based on prop changes. The `componentWillReceiveProps` lifecycle method is deprecated and can lead to unexpected behavior. This example shows how to correctly update state using the recommended `getDerivedStateFromProps` or `componentDidUpdate` methods.

## Bug Description

The original code uses `componentWillReceiveProps`, which is deprecated.  This can lead to inconsistent state updates and unexpected behavior, particularly with concurrent rendering modes.  The solution shows how to refactor the code to use either `getDerivedStateFromProps` or `componentDidUpdate` for proper state management.

## Solution

The solution demonstrates how to refactor the component to use `getDerivedStateFromProps` or `componentDidUpdate` for correctly handling prop updates and preventing potential bugs.