## CPP

### SOLUTION

int lowestCommonAncestorValue(TreeNode* root, int p, int q) {
    if (!root) return -1;

    if (root->val == p || root->val == q)
        return root->val;

    int left = lowestCommonAncestorValue(root->left, p, q);
    int right = lowestCommonAncestorValue(root->right, p, q);

    if (left != -1 && right != -1)
        return root->val;

    return left != -1 ? left : right;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512



## JAVA

### SOLUTION

public static int lowestCommonAncestorValue(TreeNode root, int p, int q) {
    if (root == null) return -1;

    if (root.val == p || root.val == q)
        return root.val;

    int left = lowestCommonAncestorValue(root.left, p, q);
    int right = lowestCommonAncestorValue(root.right, p, q);

    if (left != -1 && right != -1)
        return root.val;

    return left != -1 ? left : right;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512



## C

### SOLUTION

int lowestCommonAncestorValue(struct TreeNode* root, int p, int q) {
    if (root == NULL) return -1;

    if (root->val == p || root->val == q)
        return root->val;

    int left = lowestCommonAncestorValue(root->left, p, q);
    int right = lowestCommonAncestorValue(root->right, p, q);

    if (left != -1 && right != -1)
        return root->val;

    return left != -1 ? left : right;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512



## JAVASCRIPT

### SOLUTION

function lowestCommonAncestorValue(root, p, q) {
    if (!root) return -1;

    if (root.val === p || root.val === q)
        return root.val;

    const left = lowestCommonAncestorValue(root.left, p, q);
    const right = lowestCommonAncestorValue(root.right, p, q);

    if (left !== -1 && right !== -1)
        return root.val;

    return left !== -1 ? left : right;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512



## PYTHON

### SOLUTION

def lowest_common_ancestor_value(root: TreeNode, p: int, q: int) -> int:
    if not root:
        return -1

    if root.val == p or root.val == q:
        return root.val

    left = lowest_common_ancestor_value(root.left, p, q)
    right = lowest_common_ancestor_value(root.right, p, q)

    if left != -1 and right != -1:
        return root.val

    return left if left != -1 else right

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512