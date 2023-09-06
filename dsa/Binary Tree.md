## Structure
```ts
type BinaryTree = {
  value: number;
  left?: BinaryTree;
  right?: BinaryTree;
}
```

## Patterns
### Pre-Order Traversal
```ts
const traverse = (
  root: BinaryTree|undefined,
  visitNode: (node: number) => void
) => {
  if (root) {
    visitNode(root.value);
    traverse(root.left, visitNode);
    traverse(root.right, visitNode);
  }
}
```

### In-Order Traversal
Same as pre-order but with the `visitNode` in between the `traverse` calls.
### Post-Order Traversal
Same as pre-order but with the `visitNode` after the `traverse` calls.