## CPP

### SOLUTION

long long solveQuantumSignal(int n, vector<int>& arr) {
    long long res = 0;
    long long MOD = 998244353;
    
    for(int i = 0; i < 31; ++i) {
        long long one = 0;
        
        long long freqCount[2] = {0, 0};
        long long freqSum[2] = {0, 0};
        
        freqCount[0] = 1;
        freqSum[0] = -1;
        
        long long current_bit_contribution = 0;
        
        for(int j = 0; j < n; ++j) {
            if((arr[j] >> i) & 1) {
                one++;
            }
            
            int current_parity = one % 2;
            int required_prev_parity = 1 - current_parity; 
            
            long long count = freqCount[required_prev_parity];
            long long sum_indices = freqSum[required_prev_parity];
            
            long long term = (count * j - sum_indices) % MOD;
            current_bit_contribution = (current_bit_contribution + term) % MOD;
            
            freqCount[current_parity]++;
            freqSum[current_parity] += j;
        }
        
        long long bit_val = (1LL << i) % MOD;
        res = (res + current_bit_contribution * bit_val) % MOD;
    }
    
    return (res + MOD) % MOD;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public long solveQuantumSignal(int n, int[] arr) {
    long res = 0;
    long MOD = 998244353;
    
    for (int i = 0; i < 31; ++i) {
        long one = 0;
    
        long[][] freq = new long[2][2];
        
        freq[0][0] = 1; 
        freq[0][1] = -1;
        
        long currentBitContribution = 0;
        
        for (int j = 0; j < n; ++j) {
            if (((arr[j] >> i) & 1) == 1) {
                one++;
            }
            
            int currentParity = (int)(one % 2);
            int targetParity = 1 - currentParity;
            
            long count = freq[targetParity][0];
            long sumIndices = freq[targetParity][1];
            
            long term = (count * j - sumIndices) % MOD;
            currentBitContribution = (currentBitContribution + term) % MOD;
            
            freq[currentParity][0]++;
            freq[currentParity][1] += j;
        }
        
        long bitVal = (1L << i) % MOD;
        res = (res + currentBitContribution * bitVal) % MOD;
    }
    
    return (res + MOD) % MOD;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

