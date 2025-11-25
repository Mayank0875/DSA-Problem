## CPP

### SOLUTION

vector<int> zigZagTraversal(TreeNode* root) {
    vector<int> result;
    if (!root) return result;

    queue<TreeNode*> q;
    q.push(root);
    bool leftToRight = true;

    while (!q.empty()) {
        int size = q.size();
        vector<int> level;
        
        for (int i = 0; i < size; i++) {
            TreeNode* node = q.front();
            q.pop();
            level.push_back(node->val);

            if (node->left) q.push(node->left);
            if (node->right) q.push(node->right);
        }

        if (!leftToRight) {
            reverse(level.begin(), level.end());
        }

        for (int val : level) {
            result.push_back(val);
        }

        leftToRight = !leftToRight;
    }
    return result;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512



## JAVA

### SOLUTION

public static ArrayList<Integer> zigZagTraversal(TreeNode root) {
    ArrayList<Integer> result = new ArrayList<>();
    if (root == null) return result;

    Queue<TreeNode> q = new LinkedList<>();
    q.add(root);
    boolean leftToRight = true;

    while (!q.isEmpty()) {
        int size = q.size();
        ArrayList<Integer> level = new ArrayList<>();

        for (int i = 0; i < size; i++) {
            TreeNode node = q.poll();
            level.add(node.val);

            if (node.left != null) q.add(node.left);
            if (node.right != null) q.add(node.right);
        }

        if (!leftToRight) {
            Collections.reverse(level);
        }

        result.addAll(level);
        leftToRight = !leftToRight;
    }
    return result;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512



## C

### SOLUTION

int* zigZagTraversal(struct TreeNode* root, int* returnSize) {
    if (!root) {
        *returnSize = 0;
        return NULL;
    }

    // Estimate max nodes
    int maxNodes = 100005;
    int* result = (int*)malloc(maxNodes * sizeof(int));
    *returnSize = 0;

    struct TreeNode** queue = (struct TreeNode**)malloc(maxNodes * sizeof(struct TreeNode*));
    int front = 0, rear = 0;

    queue[rear++] = root;
    int leftToRight = 1;

    while (front < rear) {
        int levelSize = rear - front;
        int* level = (int*)malloc(levelSize * sizeof(int));

        for (int i = 0; i < levelSize; i++) {
            struct TreeNode* node = queue[front++];
            level[i] = node->val;

            if (node->left) queue[rear++] = node->left;
            if (node->right) queue[rear++] = node->right;
        }

        if (!leftToRight) {
            for (int i = 0; i < levelSize / 2; i++) {
                int temp = level[i];
                level[i] = level[levelSize - 1 - i];
                level[levelSize - 1 - i] = temp;
            }
        }

        for (int i = 0; i < levelSize; i++) {
            result[(*returnSize)++] = level[i];
        }

        free(level);
        leftToRight = !leftToRight;
    }

    free(queue);
    return result;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512



## JAVASCRIPT

### SOLUTION

function zigZagTraversal(root) {
    const result = [];
    if (!root) return result;

    const queue = [root];
    let leftToRight = true;

    while (queue.length > 0) {
        const levelSize = queue.length;
        const level = [];

        for (let i = 0; i < levelSize; i++) {
            const node = queue.shift();
            level.push(node.val);

            if (node.left) queue.push(node.left);
            if (node.right) queue.push(node.right);
        }

        if (!leftToRight) {
            level.reverse();
        }

        result.push(...level);
        leftToRight = !leftToRight;
    }
    return result;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512



## PYTHON

### SOLUTION


def zig_zag_traversal(root: TreeNode) -> list:
    if not root:
        return []
    
    result = []
    queue = collections.deque([root])
    left_to_right = True
    
    while queue:
        level_size = len(queue)
        level = []
        
        for _ in range(level_size):
            node = queue.popleft()
            level.append(node.val)
            
            if node.left:
                queue.append(node.left)
            if node.right:
                queue.append(node.right)
        
        if not left_to_right:
            level.reverse()
            
        result.extend(level)
        left_to_right = not left_to_right
        
    return result

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512