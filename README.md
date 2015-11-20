# react-ui-tree
React tree component

This project is a fork of gqx react-ui-tree.  It uses the basis of that component but removes the drag and drop
functionality to better interact with a react dnd container.

```

build requires babel 6.x
### Installation
``` sh
npm install https://github.com/mockeryjones/yb-ui-tree.git --save
```
### Usage
``` javascript
<Tree
  paddingLeft={20}              // left padding for children nodes in pixels
  tree={this.state.tree}        // tree object
  onChange={this.handleChange}  // onChange(tree) tree object changed
  renderNode={this.renderNode}  // renderNode(node) return react element
/>

// a sample tree object
// node.children, node.collapsed, node.leaf properties are hardcoded
{
  "module": "react-ui-tree",
  "children": [{
    "collapsed": true,
    "module": "dist",
    "children": [{
      "module": "node.js"
    }]
  }]
}
```
### License
MIT
