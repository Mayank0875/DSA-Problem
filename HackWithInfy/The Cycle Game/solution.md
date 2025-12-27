## CPP

### SOLUTION

long long calculateFinalScore(int n, std::vector<int> per) {
    std::vector<std::pair<long long, long long>> odd_cycles;
    std::vector<bool> used(n, true);
    long long ans = 0;

    for(int& x : per) x--;

    for (int i = 0; i < n; i++) {
        if (used[i]) {
            int curr = i;
            long long s1 = 0, s2 = 0;
            int count = 0;
            
            while (used[curr]) {
                used[curr] = false;
                if (count % 2 == 1) s2 += (curr + 1);
                else s1 += (curr + 1);
                count++;
                curr = per[curr]; 
            }

            if (count % 2 == 0) {

                if (s1 < s2) std::swap(s1, s2);
                ans += (s1 - s2);
            } else {
                std::vector<int> cycle_vals;
                curr = i; // Reconstruct cycle to iterate rotations
            
                int start_node = i;
                std::vector<int> b;
                b.push_back(start_node + 1);
                int y = per[start_node];
                while(y != start_node){
                    b.push_back(y + 1);
                    y = per[y];
                }

                long long current_s1 = 0, current_s2 = 0;
                for(int j=0; j<count; ++j){
                    if(j % 2 != 0) current_s2 += b[j];
                    else current_s1 += b[j];
                }

                long long best_s1 = current_s1, best_s2 = current_s2;
                
            
                for(int j=0; j<count; ++j){
                    int val = b[j];
                    if(j % 2 != 0) { // val was in s2
                        current_s2 -= val;
                        current_s1 += val;
                        if(current_s1 > best_s1) {
                             best_s1 = current_s1;
                             best_s2 = current_s2;
                        }
                    } else { // val was in s1
                        current_s1 -= val;
                        current_s2 += val;
                        if(current_s2 > best_s1) { // Compare against current best 's1'
                             best_s1 = current_s2;
                             best_s2 = current_s1;
                        }
                    }
                }
                odd_cycles.push_back({best_s1, best_s2});
            }
        }
    }

    std::sort(odd_cycles.begin(), odd_cycles.end(), 
        [](const std::pair<long long, long long>& a, const std::pair<long long, long long>& b) {
            return (a.first - a.second) > (b.first - b.second);
        }
    );

    for (size_t i = 0; i < odd_cycles.size(); i++) {
        if (i % 2 == 0) {
            ans += odd_cycles[i].first;
            ans -= odd_cycles[i].second;
        } else {
            ans -= odd_cycles[i].first;
            ans += odd_cycles[i].second;
        }
    }

    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long calculateFinalScore(int n, int[] p) {
    ArrayList<long[]> oddCycles = new ArrayList<>();
    boolean[] used = new boolean[n];
    long ans = 0;

    for (int i = 0; i < n; i++) p[i]--;

    for (int i = 0; i < n; i++) {
        if (!used[i]) {
            int curr = i;
            long s1 = 0, s2 = 0;
            int count = 0;

            while (!used[curr]) {
                used[curr] = true;
                if ((count & 1) == 1) s2 += (curr + 1);
                else s1 += (curr + 1);
                count++;
                curr = p[curr];
            }

            if ((count & 1) == 0) {
                // Even cycle
                if (s1 < s2) { long temp = s1; s1 = s2; s2 = temp; }
                ans += (s1 - s2);
            } else {
                ArrayList<Integer> b = new ArrayList<>();
                int startNode = i; // This was the start of this traversal
                b.add(startNode + 1);
                int y = p[startNode];
                while (y != startNode) {
                    b.add(y + 1);
                    y = p[y];
                }

                long currS1 = 0, currS2 = 0;
                for (int j = 0; j < count; j++) {
                    if ((j & 1) == 1) currS2 += b.get(j);
                    else currS1 += b.get(j);
                }

                long bestS1 = currS1, bestS2 = currS2;

                for (int j = 0; j < count; j++) {
                    int val = b.get(j);
                    if ((j & 1) == 1) {
                        currS2 -= val;
                        currS1 += val;
                        if (currS1 > bestS1) {
                            bestS1 = currS1;
                            bestS2 = currS2;
                        }
                    } else {
                        currS1 -= val;
                        currS2 += val;
                        if (currS2 > bestS1) {
                            bestS1 = currS2;
                            bestS2 = currS1;
                        }
                    }
                }
                oddCycles.add(new long[]{bestS1, bestS2});
            }
        }
    }

    oddCycles.sort((a, b) -> Long.compare((b[0] - b[1]), (a[0] - a[1])));

    for (int i = 0; i < oddCycles.size(); i++) {
        if ((i & 1) == 0) {
            ans += oddCycles.get(i)[0];
            ans -= oddCycles.get(i)[1];
        } else {
            ans -= oddCycles.get(i)[0];
            ans += oddCycles.get(i)[1];
        }
    }

    return ans;
}

### METADATA

**TimeLimit**  
3000  

**MemoryLimit**  
512  
