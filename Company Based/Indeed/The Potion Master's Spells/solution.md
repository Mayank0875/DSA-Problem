## CPP
### SOLUTION
int countValidSpells(vector<string>& words, string runes) {
    vector<int> runeCounts(26, 0);
    for (char c : runes) {
        runeCounts[c - 'a']++;
    }

    int totalPower = 0;

    for (const string& word : words) {
        vector<int> wordCounts(26, 0);
        bool possible = true;

        for (char c : word) {
            wordCounts[c - 'a']++;
        }

        for (int i = 0; i < 26; i++) {
            if (wordCounts[i] > runeCounts[i]) {
                possible = false;
                break;
            }
        }

        if (possible) {
            totalPower += word.length();
        }
    }

    return totalPower;
}

### METADATA
**TimeLimit**
1000
**MemoryLimit**
256000

## JAVA
### SOLUTION
public static int countValidSpells(String[] words, String runes) {
    int[] runeCounts = new int[26];
    for (char c : runes.toCharArray()) {
        runeCounts[c - 'a']++;
    }

    int totalPower = 0;

    for (String word : words) {
        int[] wordCounts = new int[26];
        boolean possible = true;

        for (char c : word.toCharArray()) {
            wordCounts[c - 'a']++;
        }

        for (int i = 0; i < 26; i++) {
            if (wordCounts[i] > runeCounts[i]) {
                possible = false;
                break;
            }
        }

        if (possible) {
            totalPower += word.length();
        }
    }

    return totalPower;
}

### METADATA
**TimeLimit**
1000
**MemoryLimit**
256000

## C
### SOLUTION
int countValidSpells(int n, char** words, char* runes) {
    int runeCounts[26] = {0};
    for (int i = 0; runes[i] != '\0'; i++) {
        runeCounts[runes[i] - 'a']++;
    }

    int totalPower = 0;

    for (int i = 0; i < n; i++) {
        int wordCounts[26] = {0};
        int possible = 1;
        int len = 0;

        for (int j = 0; words[i][j] != '\0'; j++) {
            wordCounts[words[i][j] - 'a']++;
            len++;
        }

        for (int k = 0; k < 26; k++) {
            if (wordCounts[k] > runeCounts[k]) {
                possible = 0;
                break;
            }
        }

        if (possible) {
            totalPower += len;
        }
    }

    return totalPower;
}

### METADATA
**TimeLimit**
1000
**MemoryLimit**
256000

## JAVASCRIPT
### SOLUTION
function countValidSpells(words, runes) {
    const runeCounts = new Array(26).fill(0);
    for (let i = 0; i < runes.length; i++) {
        runeCounts[runes.charCodeAt(i) - 97]++;
    }

    let totalPower = 0;

    for (const word of words) {
        const wordCounts = new Array(26).fill(0);
        let possible = true;

        for (let i = 0; i < word.length; i++) {
            wordCounts[word.charCodeAt(i) - 97]++;
        }

        for (let i = 0; i < 26; i++) {
            if (wordCounts[i] > runeCounts[i]) {
                possible = false;
                break;
            }
        }

        if (possible) {
            totalPower += word.length;
        }
    }

    return totalPower;
}

### METADATA
**TimeLimit**
1000
**MemoryLimit**
256000

## PYTHON
### SOLUTION
def count_valid_spells(words: list, runes: str) -> int:
    rune_counts = [0] * 26
    for char in runes:
        rune_counts[ord(char) - ord('a')] += 1
    
    total_power = 0
    
    for word in words:
        word_counts = [0] * 26
        possible = True
        for char in word:
            word_counts[ord(char) - ord('a')] += 1
        
        for i in range(26):
            if word_counts[i] > rune_counts[i]:
                possible = False
                break
        
        if possible:
            total_power += len(word)
            
    return total_power

### METADATA
**TimeLimit**
1000
**MemoryLimit**
256000